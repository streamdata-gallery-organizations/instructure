---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Calendar Events API List calendar events
  description: List calendar events.
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
  /calendar_events:
    get:
      summary: List calendar events
      description: List calendar events.
      operationId: list-calendar-events
      x-api-path-slug: calendar-events-get
      parameters:
      - in: query
        name: all_events
        description: Defaults to false (uses start_date, end_date, and undated criteria)
      - in: query
        name: context_codes[]
        description: List of context codes of courses/groups/users whose events you
          want to see
      - in: query
        name: end_date
        description: Only return events before the end_date (inclusive)
      - in: query
        name: excludes[]
        description: Array of attributes to exclude
      - in: query
        name: start_date
        description: Only return events since the start_date (inclusive)
      - in: query
        name: type
        description: 'Defaults to u201ceventu201dnn        n        n          Allowed
          values: event, assignment'
      - in: query
        name: undated
        description: Defaults to false (dated events only)
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
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