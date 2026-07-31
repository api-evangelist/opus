---
name: Clip a video and publish it to social accounts
description: >-
  Turn a long video into clips, generate platform-specific social copy, and
  publish or schedule the clips to connected social accounts.
api: openapi/opus-openapi-original.json
operations:
  - ClipProjectController_createClipProject
  - ExportableClipController_queryExportableClips
  - SocialAccountController_getSocialAccounts
  - SocialCopyJobController_createSocialCopyJob
  - SocialCopyJobController_getSocialCopyJob
  - PostTaskController_createPostTask
  - PublishScheduleController_createPublishSchedule
---

# Clip a video and publish it to social accounts

Base URL: `https://api.opus.pro`. Auth: `Authorization: Bearer <API_KEY>`.

## Steps

1. **Create the project & get clips** — `POST /api/clip-projects`
   (`ClipProjectController_createClipProject`), then
   `GET /api/exportable-clips?q=findByProjectId&projectId={projectId}`
   (`ExportableClipController_queryExportableClips`) once clipping completes.
2. **List connected accounts** — `GET /api/social-accounts`
   (`SocialAccountController_getSocialAccounts`) to pick target platforms.
3. **Generate social copy** — `POST /api/social-copy-jobs`
   (`SocialCopyJobController_createSocialCopyJob`) returns a `jobId`; poll
   `GET /api/social-copy-jobs/{jobId}` (`SocialCopyJobController_getSocialCopyJob`).
4. **Publish now** — `POST /api/post-tasks`
   (`PostTaskController_createPostTask`) to post a clip immediately. Posting to
   X consumes 1 credit per post.
   **or Schedule** — `POST /api/publish-schedules`
   (`PublishScheduleController_createPublishSchedule`) for future posting;
   cancel with `DELETE /api/publish-schedules/{scheduleId}`.

## Rules

- Social-posting endpoints have their own per-endpoint rate limits (separate
  from the 30 req/min core limit).
- Always resolve the HD/export URL for a clip before posting where required;
  list/describe return preview URLs only.
