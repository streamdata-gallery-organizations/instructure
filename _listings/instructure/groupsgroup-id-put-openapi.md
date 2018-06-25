---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Groups API Edit a group
  description: Edit a group.
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