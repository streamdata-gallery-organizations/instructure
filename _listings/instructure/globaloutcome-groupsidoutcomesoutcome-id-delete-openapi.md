---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Global API Unlink an outcome
  description: Unlink an outcome.
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
    post:
      summary: Create/link an outcome
      description: Create/link an outcome.
      operationId: createlink-an-outcome
      x-api-path-slug: globaloutcome-groupsidoutcomes-post
      parameters:
      - in: query
        name: calculation_int
        description: The new calculation int
      - in: query
        name: calculation_method
        description: The new calculation method
      - in: query
        name: description
        description: The description of the new outcome
      - in: query
        name: display_name
        description: A friendly name shown in reports for outcomes with cryptic titles,
          such asncommon core standards names
      - in: query
        name: mastery_points
        description: The mastery threshold for the embedded rubric criterion
      - in: query
        name: outcome_id
        description: The ID of the existing outcome to link
      - in: query
        name: ratings[][description]
        description: The description of a rating level for the embedded rubric criterion
      - in: query
        name: ratings[][points]
        description: The points corresponding to a rating level for the embedded rubricncriterion
      - in: query
        name: title
        description: The title of the new outcome
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
      - Outcomes
  /global/outcome_groups/{id}/outcomes/outcome_id:
    delete:
      summary: Unlink an outcome
      description: Unlink an outcome.
      operationId: unlink-an-outcome
      x-api-path-slug: globaloutcome-groupsidoutcomesoutcome-id-delete
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
      - Outcomes
      - Outcome
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