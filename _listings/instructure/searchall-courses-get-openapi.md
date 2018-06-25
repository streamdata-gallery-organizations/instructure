---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Utility APIs List all courses
  description: List all courses.
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
  /api/sis/accounts/{account_id}/assignments:
    get:
      summary: Retrieve assignments enabled for grade export to SIS
      description: Retrieve assignments enabled for grade export to sis.
      operationId: retrieve-assignments-enabled-for-grade-export-to-sis
      x-api-path-slug: apisisaccountsaccount-idassignments-get
      parameters:
      - in: query
        name: account_id
        description: The ID of the account to query
      - in: query
        name: course_id
        description: The ID of the course to query
      - in: query
        name: ends_after
        description: When searching on an account, restricts to courses that end after
          this daten(if they have an end date)
      - in: query
        name: starts_before
        description: When searching on an account, restricts to courses that start
          before thisndate (if they have a start date)
      responses:
        200:
          description: OK
      tags:
      - Api
      - Sis
      - Accounts
      - Account
      - Id
      - Assignments
  /api/sis/courses/{course_id}/assignments:
    get:
      summary: Retrieve assignments enabled for grade export to SIS
      description: Retrieve assignments enabled for grade export to sis.
      operationId: retrieve-assignments-enabled-for-grade-export-to-sis
      x-api-path-slug: apisiscoursescourse-idassignments-get
      parameters:
      - in: query
        name: account_id
        description: The ID of the account to query
      - in: query
        name: course_id
        description: The ID of the course to query
      - in: query
        name: ends_after
        description: When searching on an account, restricts to courses that end after
          this daten(if they have an end date)
      - in: query
        name: starts_before
        description: When searching on an account, restricts to courses that start
          before thisndate (if they have a start date)
      responses:
        200:
          description: OK
      tags:
      - Api
      - Sis
      - Courses
      - Course
      - Id
      - Assignments
  /collaborations/{id}/members:
    get:
      summary: List members of a collaboration.
      description: List members of a collaboration..
      operationId: list-members-of-a-collaboration
      x-api-path-slug: collaborationsidmembers-get
      responses:
        200:
          description: OK
      tags:
      - Collaborations
      - Id
      - Members
  /comm_messages:
    get:
      summary: List of CommMessages for a user
      description: List of commmessages for a user.
      operationId: list-of-commmessages-for-a-user
      x-api-path-slug: comm-messages-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range you want to retrieve messages for
      - in: query
        name: start_time
        description: The beginning of the time range you want to retrieve message
          from
      - in: query
        name: user_id
        description: The user id for whom you want to retrieve CommMessages
      responses:
        200:
          description: OK
      tags:
      - Comm
      - Messages
  /course_accounts:
    get:
      summary: List accounts for course admins
      description: List accounts for course admins.
      operationId: list-accounts-for-course-admins
      x-api-path-slug: course-accounts-get
      responses:
        200:
          description: OK
      tags:
      - Course
      - Accounts
  /error_reports:
    post:
      summary: Create Error Report
      description: Create error report.
      operationId: create-error-report
      x-api-path-slug: error-reports-post
      parameters:
      - in: query
        name: error[comments]
        description: The long version of the story from the user one what they experienced
      - in: query
        name: error[email]
        description: Email address for the reporting user
      - in: query
        name: error[http_env]
        description: A collection of metadata about the users&#39; environment
      - in: query
        name: error[subject]
        description: The summary of the problem
      - in: query
        name: error[url]
        description: URL from which the report was issued
      responses:
        200:
          description: OK
      tags:
      - Error
      - Reports
  /jwts:
    post:
      summary: Create JWT
      description: Create jwt.
      operationId: create-jwt
      x-api-path-slug: jwts-post
      responses:
        200:
          description: OK
      tags:
      - Jwts
  /outcomes/{id}:
    get:
      summary: Show an outcome
      description: Show an outcome.
      operationId: show-an-outcome
      x-api-path-slug: outcomesid-get
      responses:
        200:
          description: OK
      tags:
      - Outcomes
      - Id
    put:
      summary: Update an outcome
      description: Update an outcome.
      operationId: update-an-outcome
      x-api-path-slug: outcomesid-put
      parameters:
      - in: query
        name: calculation_int
        description: The new calculation int
      - in: query
        name: calculation_method
        description: The new calculation method
      - in: query
        name: description
        description: The new outcome description
      - in: query
        name: display_name
        description: A friendly name shown in reports for outcomes with cryptic titles,
          such asncommon core standards names
      - in: query
        name: mastery_points
        description: The new mastery threshold for the embedded rubric criterion
      - in: query
        name: ratings[][description]
        description: The description of a new rating level for the embedded rubric
          criterion
      - in: query
        name: ratings[][points]
        description: The points corresponding to a new rating level for the embedded
          rubricncriterion
      - in: query
        name: title
        description: The new outcome title
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
      responses:
        200:
          description: OK
      tags:
      - Outcomes
      - Id
  /progress/{id}:
    get:
      summary: Query progress
      description: Query progress.
      operationId: query-progress
      x-api-path-slug: progressid-get
      responses:
        200:
          description: OK
      tags:
      - Progress
      - Id
  /search/all_courses:
    get:
      summary: List all courses
      description: List all courses.
      operationId: list-all-courses
      x-api-path-slug: searchall-courses-get
      parameters:
      - in: query
        name: open_enrollment_only
        description: Only return courses that allow self enrollment
      - in: query
        name: public_only
        description: Only return courses with public content
      - in: query
        name: search
        description: Search terms used for matching users/courses/groups (e
      responses:
        200:
          description: OK
      tags:
      - Search
      - ""
      - Courses
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