---
name: Clip a long video and export the best clips
description: >-
  Submit a long-form video to OpusClip, wait for clipping to finish, list the
  generated clips, and get their HD download URLs.
api: openapi/opus-openapi-original.json
operations:
  - ClipProjectController_createClipProject
  - ClipProjectController_getClipProjectDetail
  - ExportableClipController_queryExportableClips
---

# Clip a long video and export the best clips

Base URL: `https://api.opus.pro`. Auth: `Authorization: Bearer <API_KEY>` (org
API key from the dashboard). Some list calls also take `x-opus-org-id: <ORG_ID>`.

## Steps

1. **Create the project** — `POST /api/clip-projects`
   (`ClipProjectController_createClipProject`). Send `{ "videoUrl": "<youtube-or-vimeo-or-signed-upload-url>" }`.
   Optionally add `brandTemplateId`, `curationPref` (range, clipDurations,
   topicKeywords, genre), `importPref` (sourceLang), and `conclusionActions`
   (a `WEBHOOK` action to be notified when clipping completes). Returns a
   project with an `id`. Note the 10-credit per-project minimum.
2. **Wait for completion** — either receive the `WEBHOOK` conclusion action
   (verify the `X-Opus-Signature` HMAC — see `conventions/`), or poll
   `GET /api/clip-projects/{projectId}`
   (`ClipProjectController_getClipProjectDetail`) until the project is ready.
3. **List clips** — `GET /api/exportable-clips?q=findByProjectId&projectId={projectId}`
   (`ExportableClipController_queryExportableClips`), paginating with
   `pageNum` (from 1) and `pageSize`. These return preview URLs.
4. **Export** — request the HD download for the clips you want (via the
   `export_clip` / `export_collection` MCP tools, or a collection export
   `POST /api/collections/{collectionId}/export`).

## Rules

- Respect the 30 req/min rate limit (`429`) and the 900-credit monthly cap
  (`403`, body `{code: API_MONTHLY_CAP_REACHED, reset_at, upgrade_url}`) — do
  not retry a `403` in a loop.
- Concurrency: Pro Beta/Max 4, Business 50 parallel projects; over-limit `429`
  carries `X-Cap-Reason: concurrent` — back off and retry.
