---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API Update a content migration
  description: Update a content migration.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups:
    post:
      summary: Create a group
      description: Create a group.
      operationId: create-a-group
      x-api-path-slug: groups-post
      parameters:
      - in: query
        name: description
        description: A description of the group
      - in: query
        name: is_public
        description: whether the group is public (applies only to community groups)
      - in: query
        name: join_level
        description: 'no descriptionnn        n        n          Allowed values:
          parent_context_auto_join, parent_context_request, invitation_only'
      - in: query
        name: name
        description: The name of the group
      - in: query
        name: storage_quota_mb
        description: The allowed file storage for the group, in megabytes
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{group_id}:
    delete:
      summary: Delete a group
      description: Delete a group.
      operationId: delete-a-group
      x-api-path-slug: groupsgroup-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
    get:
      summary: Get a single group
      description: Get a single group.
      operationId: get-a-single-group
      x-api-path-slug: groupsgroup-id-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cpermissionsu201d: Include permissions the current user
          has for the group'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
    put:
      summary: Edit a group
      description: Edit a group.
      operationId: edit-a-group
      x-api-path-slug: groupsgroup-id-put
      parameters:
      - in: query
        name: avatar_id
        description: The id of the attachment previously uploaded to the group that
          you wouldnlike to use as the avatar image for this group
      - in: query
        name: description
        description: A description of the group
      - in: query
        name: is_public
        description: Whether the group is public (applies only to community groups)
      - in: query
        name: join_level
        description: 'no descriptionnn        n        n          Allowed values:
          parent_context_auto_join, parent_context_request, invitation_only'
      - in: query
        name: members[]
        description: An array of user ids for users you would like in the group
      - in: query
        name: name
        description: The name of the group
      - in: query
        name: storage_quota_mb
        description: The allowed file storage for the group, in megabytes
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
  /groups/{group_id}/activity_stream:
    get:
      summary: Group activity stream
      description: Group activity stream.
      operationId: group-activity-stream
      x-api-path-slug: groupsgroup-idactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Activity
      - Stream
  /groups/{group_id}/activity_stream/summary:
    get:
      summary: Group activity stream summary
      description: Group activity stream summary.
      operationId: group-activity-stream-summary
      x-api-path-slug: groupsgroup-idactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Activity
      - Stream
      - Summary
  /groups/{group_id}/assignments/assignment_id/override:
    get:
      summary: Redirect to the assignment override for a group
      description: Redirect to the assignment override for a group.
      operationId: redirect-to-the-assignment-override-for-a-group
      x-api-path-slug: groupsgroup-idassignmentsassignment-idoverride-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Assignments
      - Assignment
      - Id
      - Override
  /groups/{group_id}/conferences:
    get:
      summary: List conferences
      description: List conferences.
      operationId: list-conferences
      x-api-path-slug: groupsgroup-idconferences-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Conferences
  /groups/{group_id}/content_exports:
    get:
      summary: List content exports
      description: List content exports.
      operationId: list-content-exports
      x-api-path-slug: groupsgroup-idcontent-exports-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Exports
    post:
      summary: Export content
      description: Export content.
      operationId: export-content
      x-api-path-slug: groupsgroup-idcontent-exports-post
      parameters:
      - in: query
        name: export_type
        description: u201ccommon_cartridgeu201dnnExport the contents of the course
          in the Common Cartridge (
      - in: query
        name: skip_notifications
        description: Don&#39;t send the notifications about the export to the user
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Exports
  /groups/{group_id}/content_exports/id:
    get:
      summary: Show content export
      description: Show content export.
      operationId: show-content-export
      x-api-path-slug: groupsgroup-idcontent-exportsid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Exports
      - Id
  /groups/{group_id}/content_licenses:
    get:
      summary: List licenses
      description: List licenses.
      operationId: list-licenses
      x-api-path-slug: groupsgroup-idcontent-licenses-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Licenses
  /groups/{group_id}/content_migrations:
    get:
      summary: List content migrations
      description: List content migrations.
      operationId: list-content-migrations
      x-api-path-slug: groupsgroup-idcontent-migrations-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
    post:
      summary: Create a content migration
      description: Create a content migration.
      operationId: create-a-content-migration
      x-api-path-slug: groupsgroup-idcontent-migrations-post
      parameters:
      - in: query
        name: date_shift_options[day_substitutions][X]
        description: Move anything scheduled for day &#39;X&#39; to the specified
          day
      - in: query
        name: date_shift_options[new_end_date]
        description: The new end date for the source content/course
      - in: query
        name: date_shift_options[new_start_date]
        description: The new start date for the content/course
      - in: query
        name: date_shift_options[old_end_date]
        description: The original end date of the source content/course
      - in: query
        name: date_shift_options[old_start_date]
        description: The original start date of the source content/course
      - in: query
        name: date_shift_options[remove_dates]
        description: Whether to remove dates in the copied course
      - in: query
        name: date_shift_options[shift_dates]
        description: Whether to shift dates in the copied course
      - in: query
        name: migration_type
        description: The type of the migration
      - in: query
        name: pre_attachment[*]
        description: Other file upload properties, See File Upload Documentation
      - in: query
        name: pre_attachment[name]
        description: Required if uploading a file
      - in: query
        name: settings[file_url]
        description: A URL to download the file from
      - in: query
        name: settings[folder_id]
        description: 'The folder to unzip the '
      - in: query
        name: settings[overwrite_quizzes]
        description: Whether to overwrite quizzes with the same identifiers between
          contentnpackages
      - in: query
        name: settings[question_bank_id]
        description: The existing question bank ID to import questions into if not
          specified innthe content package
      - in: query
        name: settings[question_bank_name]
        description: The question bank to import questions into if not specified in
          the contentnpackage, if both bank id and name are set, id will take precedence
      - in: query
        name: settings[source_course_id]
        description: The course to copy from for a course copy migration
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
  /groups/{group_id}/content_migrations/content_migration_id/migration_issues:
    get:
      summary: List migration issues
      description: List migration issues.
      operationId: list-migration-issues
      x-api-path-slug: groupsgroup-idcontent-migrationscontent-migration-idmigration-issues-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
  /groups/{group_id}/content_migrations/content_migration_id/migration_issues/{id}:
    get:
      summary: Get a migration issue
      description: Get a migration issue.
      operationId: get-a-migration-issue
      x-api-path-slug: groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
      - Id
    put:
      summary: Update a migration issue
      description: Update a migration issue.
      operationId: update-a-migration-issue
      x-api-path-slug: groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-put
      parameters:
      - in: query
        name: workflow_state
        description: Set the workflow_state of the issue
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
      - Id
  /groups/{group_id}/content_migrations/id:
    get:
      summary: Get a content migration
      description: Get a content migration.
      operationId: get-a-content-migration
      x-api-path-slug: groupsgroup-idcontent-migrationsid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Id
    put:
      summary: Update a content migration
      description: Update a content migration.
      operationId: update-a-content-migration
      x-api-path-slug: groupsgroup-idcontent-migrationsid-put
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Id
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---