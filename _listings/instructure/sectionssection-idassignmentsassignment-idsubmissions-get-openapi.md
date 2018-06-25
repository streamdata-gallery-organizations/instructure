---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Sections API List assignment submissions
  description: List assignment submissions.
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
  /sections/{course_section_id}/assignments/assignment_id/override:
    get:
      summary: Redirect to the assignment override for a section
      description: Redirect to the assignment override for a section.
      operationId: redirect-to-the-assignment-override-for-a-section
      x-api-path-slug: sectionscourse-section-idassignmentsassignment-idoverride-get
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Course
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Override
  /sections/{id}:
    delete:
      summary: Delete a section
      description: Delete a section.
      operationId: delete-a-section
      x-api-path-slug: sectionsid-delete
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Id
    get:
      summary: Get section information
      description: Get section information.
      operationId: get-section-information
      x-api-path-slug: sectionsid-get
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Id
    put:
      summary: Edit a section
      description: Edit a section.
      operationId: edit-a-section
      x-api-path-slug: sectionsid-put
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Id
  /sections/{id}/crosslist:
    delete:
      summary: De-cross-list a Section
      description: De-cross-list a section.
      operationId: decrosslist-a-section
      x-api-path-slug: sectionsidcrosslist-delete
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Id
      - Crosslist
  /sections/{id}/crosslist/new_course_id:
    post:
      summary: Cross-list a Section
      description: Cross-list a section.
      operationId: crosslist-a-section
      x-api-path-slug: sectionsidcrosslistnew-course-id-post
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Id
      - Crosslist
      - New
      - Course
      - Id
  /sections/{section_id}/assignments/assignment_id/peer_reviews:
    get:
      summary: Get all Peer Reviews
      description: Get all peer reviews.
      operationId: get-all-peer-reviews
      x-api-path-slug: sectionssection-idassignmentsassignment-idpeer-reviews-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the peer review
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Peer
      - Reviews
  /sections/{section_id}/assignments/assignment_id/submissions:
    get:
      summary: List assignment submissions
      description: List assignment submissions.
      operationId: list-assignment-submissions
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissions-get
      parameters:
      - in: query
        name: grouped
        description: If this argument is true, the response will be grouped by student
          groups
      - in: query
        name: include[]
        description: Associations to include with the group
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
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