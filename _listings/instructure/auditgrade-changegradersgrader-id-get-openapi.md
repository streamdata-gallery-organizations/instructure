---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Audit API Query by grader.
  description: Query by grader..
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
  /audit/authentication/accounts/{account_id}:
    get:
      summary: Query by account.
      description: Query by account..
      operationId: query-by-account
      x-api-path-slug: auditauthenticationaccountsaccount-id-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want events
      - in: query
        name: start_time
        description: The beginning of the time range from which you want events
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Authentication
      - Accounts
      - Account
      - Id
  /audit/authentication/logins/{login_id}:
    get:
      summary: Query by login.
      description: Query by login..
      operationId: query-by-login
      x-api-path-slug: auditauthenticationloginslogin-id-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want events
      - in: query
        name: start_time
        description: The beginning of the time range from which you want events
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Authentication
      - Logins
      - Login
      - Id
  /audit/authentication/users/{user_id}:
    get:
      summary: Query by user.
      description: Query by user..
      operationId: query-by-user
      x-api-path-slug: auditauthenticationusersuser-id-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want events
      - in: query
        name: start_time
        description: The beginning of the time range from which you want events
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Authentication
      - Users
      - User
      - Id
  /audit/course/courses/{course_id}:
    get:
      summary: Query by course.
      description: Query by course..
      operationId: query-by-course
      x-api-path-slug: auditcoursecoursescourse-id-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want events
      - in: query
        name: start_time
        description: The beginning of the time range from which you want events
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Course
      - Courses
      - Course
      - Id
  /audit/grade_change/assignments/{assignment_id}:
    get:
      summary: Query by assignment.
      description: Query by assignment..
      operationId: query-by-assignment
      x-api-path-slug: auditgrade-changeassignmentsassignment-id-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want events
      - in: query
        name: start_time
        description: The beginning of the time range from which you want events
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Grade
      - Change
      - Assignments
      - Assignment
      - Id
  /audit/grade_change/courses/{course_id}:
    get:
      summary: Query by course.
      description: Query by course..
      operationId: query-by-course
      x-api-path-slug: auditgrade-changecoursescourse-id-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want events
      - in: query
        name: start_time
        description: The beginning of the time range from which you want events
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Grade
      - Change
      - Courses
      - Course
      - Id
  /audit/grade_change/graders/{grader_id}:
    get:
      summary: Query by grader.
      description: Query by grader..
      operationId: query-by-grader
      x-api-path-slug: auditgrade-changegradersgrader-id-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want events
      - in: query
        name: start_time
        description: The beginning of the time range from which you want events
      responses:
        200:
          description: OK
      tags:
      - Audit
      - Grade
      - Change
      - Graders
      - Grader
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