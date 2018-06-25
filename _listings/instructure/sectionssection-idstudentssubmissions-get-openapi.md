---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Sections API List submissions for multiple assignments
  description: List submissions for multiple assignments.
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
    post:
      summary: Submit an assignment
      description: Submit an assignment.
      operationId: submit-an-assignment
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissions-post
      parameters:
      - in: query
        name: comment[text_comment]
        description: Include a textual comment with the submission
      - in: query
        name: submission[body]
        description: Submit the assignment as an HTML document snippet
      - in: query
        name: submission[file_ids][]
        description: Submit the assignment as a set of one or more previously uploaded
          filesnresiding in the submitting user&#39;s files section (or the group&#39;snfiles
          section, for group assignments)
      - in: query
        name: submission[media_comment_id]
        description: The media comment id to submit
      - in: query
        name: submission[media_comment_type]
        description: The type of media comment being submitted
      - in: query
        name: submission[submission_type]
        description: The type of submission being made
      - in: query
        name: submission[url]
        description: Submit the assignment as a URL
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
  /sections/{section_id}/assignments/assignment_id/submissions/update_grades:
    post:
      summary: Grade or comment on multiple submissions
      description: Grade or comment on multiple submissions.
      operationId: grade-or-comment-on-multiple-submissions
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsupdate-grades-post
      parameters:
      - in: query
        name: grade_data[student_id][file_ids][]
        description: See documentation for the comment[] arguments in thenSubmissions
          Update documentation
      - in: query
        name: grade_data[student_id][group_comment]
        description: no description
      - in: query
        name: grade_data[student_id][media_comment_id]
        description: no description
      - in: query
        name: grade_data[student_id][media_comment_type]
        description: 'no descriptionnn        n        n          Allowed values:
          audio, video'
      - in: query
        name: grade_data[student_id][posted_grade]
        description: See documentation for the posted_grade argument in thenSubmissions
          Update documentation
      - in: query
        name: grade_data[student_id][rubric_assessment]
        description: See documentation for the rubric_assessment argument in thenSubmissions
          Update documentation
      - in: query
        name: grade_data[student_id][text_comment]
        description: no description
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
      - Update
      - Grades
  /sections/{section_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews:
    delete:
      summary: Create Peer Review
      description: Create peer review.
      operationId: create-peer-review
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete
      parameters:
      - in: query
        name: user_id
        description: user_id to delete as reviewer on this assignment
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
      - Submission
      - Id
      - Peer
      - Reviews
    get:
      summary: Get all Peer Reviews
      description: Get all peer reviews.
      operationId: get-all-peer-reviews
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get
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
      - Submissions
      - Submission
      - Id
      - Peer
      - Reviews
    post:
      summary: Create Peer Review
      description: Create peer review.
      operationId: create-peer-review
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post
      parameters:
      - in: query
        name: user_id
        description: user_id to assign as reviewer on this assignment
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
      - Submission
      - Id
      - Peer
      - Reviews
  /sections/{section_id}/assignments/assignment_id/submissions/{user_id}:
    get:
      summary: Get a single submission
      description: Get a single submission.
      operationId: get-a-single-submission
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-id-get
      parameters:
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
      - User
      - Id
    put:
      summary: Grade or comment on a submission
      description: Grade or comment on a submission.
      operationId: grade-or-comment-on-a-submission
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-id-put
      parameters:
      - in: query
        name: comment[file_ids][]
        description: Attach files to this comment that were previously uploaded using
          thenSubmission Comment API&#39;s files action
      - in: query
        name: comment[group_comment]
        description: Whether or not this comment should be sent to the entire group
          (defaults tonfalse)
      - in: query
        name: comment[media_comment_id]
        description: Add an audio/video comment to the submission
      - in: query
        name: comment[media_comment_type]
        description: The type of media comment being added
      - in: query
        name: comment[text_comment]
        description: Add a textual comment to the submission
      - in: query
        name: include[visibility]
        description: Whether this assignment is visible to the owner of the submission
      - in: query
        name: rubric_assessment
        description: Assign a rubric assessment to this assignment submission
      - in: query
        name: submission[excuse]
        description: Sets the u201cexcusedu201d status of an assignment
      - in: query
        name: submission[posted_grade]
        description: Assign a score to the submission, updating both the u201cscoreu201d
          and u201cgradeu201dnfields on the submission record
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
      - User
      - Id
  /sections/{section_id}/assignments/assignment_id/submissions/{user_id}/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-idfiles-post
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
      - User
      - Id
      - Files
  /sections/{section_id}/assignments/assignment_id/submissions/{user_id}/read:
    delete:
      summary: Mark submission as unread
      description: Mark submission as unread.
      operationId: mark-submission-as-unread
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-idread-delete
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
      - User
      - Id
      - Read
    put:
      summary: Mark submission as read
      description: Mark submission as read.
      operationId: mark-submission-as-read
      x-api-path-slug: sectionssection-idassignmentsassignment-idsubmissionsuser-idread-put
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
      - User
      - Id
      - Read
  /sections/{section_id}/enrollments:
    get:
      summary: List enrollments
      description: List enrollments.
      operationId: list-enrollments
      x-api-path-slug: sectionssection-idenrollments-get
      parameters:
      - in: query
        name: grading_period_id
        description: Return grades for the given grading_period
      - in: query
        name: role[]
        description: A list of enrollment roles to return
      - in: query
        name: state[]
        description: Filter by enrollment state
      - in: query
        name: type[]
        description: A list of enrollment types to return
      - in: query
        name: user_id
        description: Filter by user_id (only valid for course or section enrollment
          queries)
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Enrollments
    post:
      summary: Enroll a user
      description: Enroll a user.
      operationId: enroll-a-user
      x-api-path-slug: sectionssection-idenrollments-post
      parameters:
      - in: query
        name: enrollment[course_section_id]
        description: The ID of the course section to enroll the student in
      - in: query
        name: enrollment[enrollment_state]
        description: If set to &#39;active,&#39; student will be immediately enrolled
          in thencourse
      - in: query
        name: enrollment[limit_privileges_to_course_section]
        description: If set, the enrollment will only allow the user to see and interact
          withnusers enrolled in the section given by course_section_id
      - in: query
        name: enrollment[notify]
        description: If true, a notification will be sent to the enrolled user
      - in: query
        name: enrollment[role]
        description: Assigns a custom course-level role to the user
      - in: query
        name: enrollment[role_id]
        description: Assigns a custom course-level role to the user
      - in: query
        name: enrollment[self_enrolled]
        description: If true, marks the enrollment as a self-enrollment, which gives
          studentsnthe ability to drop the course if desired
      - in: query
        name: enrollment[self_enrollment_code]
        description: If the current user is not allowed to manage enrollments in this
          course,nbut the course allows self-enrollment, the user can self- enroll
          as anstudent in the default section by passing in a valid code
      - in: query
        name: enrollment[type]
        description: Enroll the user as a student, teacher, TA, observer, or designer
      - in: query
        name: enrollment[user_id]
        description: The ID of the user to be enrolled in the course
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Enrollments
  /sections/{section_id}/students/submissions:
    get:
      summary: List submissions for multiple assignments
      description: List submissions for multiple assignments.
      operationId: list-submissions-for-multiple-assignments
      x-api-path-slug: sectionssection-idstudentssubmissions-get
      parameters:
      - in: query
        name: assignment_ids[]
        description: List of assignments to return submissions for
      - in: query
        name: grading_period_id
        description: The id of the grading period in which submissions are being requestedn(Requires
          the Multiple Grading Periods account feature turned on)
      - in: query
        name: grouped
        description: If this argument is present, the response will be grouped by
          student,nrather than a flat array of submissions
      - in: query
        name: include[]
        description: Associations to include with the group
      - in: query
        name: student_ids[]
        description: List of student ids to return submissions for
      responses:
        200:
          description: OK
      tags:
      - Sections
      - Section
      - Id
      - Students
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