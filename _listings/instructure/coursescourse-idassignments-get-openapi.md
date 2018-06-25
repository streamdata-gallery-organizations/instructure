---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API List assignments
  description: List assignments.
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
  /courses:
    get:
      summary: List your courses
      description: List your courses.
      operationId: list-your-courses
      x-api-path-slug: courses-get
      parameters:
      - in: query
        name: enrollment_role
        description: Deprecated When set, only return courses where the user is enrolled
          withnthe specified course-level role
      - in: query
        name: enrollment_role_id
        description: When set, only return courses where the user is enrolled with
          the specifiedncourse-level role
      - in: query
        name: enrollment_type
        description: When set, only return courses where the user is enrolled as this
          type
      - in: query
        name: include[]
        description: 'u201cneeds_grading_countu201d: Optional information to include
          with each Course'
      - in: query
        name: state[]
        description: If set, only return courses that are in the given state(s)
      responses:
        200:
          description: OK
      tags:
      - Courses
  /courses/{course_id}/activity_stream:
    get:
      summary: Course activity stream
      description: Course activity stream.
      operationId: course-activity-stream
      x-api-path-slug: coursescourse-idactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Activity
      - Stream
  /courses/{course_id}/activity_stream/summary:
    get:
      summary: Course activity stream summary
      description: Course activity stream summary.
      operationId: course-activity-stream-summary
      x-api-path-slug: coursescourse-idactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Activity
      - Stream
      - Summary
  /courses/{course_id}/analytics/activity:
    get:
      summary: Get course-level participation data
      description: Get course-level participation data.
      operationId: get-courselevel-participation-data
      x-api-path-slug: coursescourse-idanalyticsactivity-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Activity
  /courses/{course_id}/analytics/assignments:
    get:
      summary: Get course-level assignment data
      description: Get course-level assignment data.
      operationId: get-courselevel-assignment-data
      x-api-path-slug: coursescourse-idanalyticsassignments-get
      parameters:
      - in: query
        name: async
        description: If async is true, then the course_assignments call can happen
          asynch-nronously and MAY return a response containing a progress_url key
          instead ofnan assignments array
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Assignments
  /courses/{course_id}/analytics/student_summaries:
    get:
      summary: Get course-level student summary data
      description: Get course-level student summary data.
      operationId: get-courselevel-student-summary-data
      x-api-path-slug: coursescourse-idanalyticsstudent-summaries-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Student
      - Summaries
  /courses/{course_id}/analytics/users/student_id/activity:
    get:
      summary: Get user-in-a-course-level participation data
      description: Get user-in-a-course-level participation data.
      operationId: get-userinacourselevel-participation-data
      x-api-path-slug: coursescourse-idanalyticsusersstudent-idactivity-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Users
      - Student
      - Id
      - Activity
  /courses/{course_id}/analytics/users/student_id/assignments:
    get:
      summary: Get user-in-a-course-level assignment data
      description: Get user-in-a-course-level assignment data.
      operationId: get-userinacourselevel-assignment-data
      x-api-path-slug: coursescourse-idanalyticsusersstudent-idassignments-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Users
      - Student
      - Id
      - Assignments
  /courses/{course_id}/analytics/users/student_id/communication:
    get:
      summary: Get user-in-a-course-level messaging data
      description: Get user-in-a-course-level messaging data.
      operationId: get-userinacourselevel-messaging-data
      x-api-path-slug: coursescourse-idanalyticsusersstudent-idcommunication-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Analytics
      - Users
      - Student
      - Id
      - Communication
  /courses/{course_id}/assignments:
    get:
      summary: List assignments
      description: List assignments.
      operationId: list-assignments
      x-api-path-slug: coursescourse-idassignments-get
      parameters:
      - in: query
        name: bucket
        description: If included, only return certain assignments depending on due
          date andnsubmission status
      - in: query
        name: include[]
        description: Associations to include with the assignment
      - in: query
        name: needs_grading_count_by_section
        description: Split up u201cneeds_grading_countu201d by sections into thenu201cneeds_grading_count_by_sectionu201d
          key, defaults to false
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides for each assignment, defaults to true
      - in: query
        name: search_term
        description: The partial title of the assignments to match and return
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
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