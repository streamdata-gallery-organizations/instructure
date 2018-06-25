---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Global API List linked outcomes
  description: List linked outcomes.
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
  /global/outcome_groups/{id}:
    delete:
      summary: Delete an outcome group
      description: Delete an outcome group.
      operationId: delete-an-outcome-group
      x-api-path-slug: globaloutcome-groupsid-delete
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
    get:
      summary: Show an outcome group
      description: Show an outcome group.
      operationId: show-an-outcome-group
      x-api-path-slug: globaloutcome-groupsid-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
    put:
      summary: Update an outcome group
      description: Update an outcome group.
      operationId: update-an-outcome-group
      x-api-path-slug: globaloutcome-groupsid-put
      parameters:
      - in: query
        name: description
        description: The new outcome group description
      - in: query
        name: parent_outcome_group_id
        description: The id of the new parent outcome group
      - in: query
        name: title
        description: The new outcome group title
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
  /global/outcome_groups/{id}/import:
    post:
      summary: Import an outcome group
      description: Import an outcome group.
      operationId: import-an-outcome-group
      x-api-path-slug: globaloutcome-groupsidimport-post
      parameters:
      - in: query
        name: source_outcome_group_id
        description: The ID of the source outcome group
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
      - Import
  /global/outcome_groups/{id}/outcomes:
    get:
      summary: List linked outcomes
      description: List linked outcomes.
      operationId: list-linked-outcomes
      x-api-path-slug: globaloutcome-groupsidoutcomes-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
      - Outcomes
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