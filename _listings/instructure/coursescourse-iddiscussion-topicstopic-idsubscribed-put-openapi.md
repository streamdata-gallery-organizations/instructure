---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Subscribe to a topic
  description: Subscribe to a topic.
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
    post:
      summary: Create an assignment
      description: Create an assignment.
      operationId: create-an-assignment
      x-api-path-slug: coursescourse-idassignments-post
      parameters:
      - in: query
        name: assignment[allowed_extensions][]
        description: 'Allowed extensions if submission_types includes u201conline_uploadu201dnnExample:nnallowed_extensions:
          [&quot;docx&quot;,&quot;ppt&quot;]'
      - in: query
        name: assignment[assignment_group_id]
        description: The assignment group id to put the assignment in
      - in: query
        name: assignment[assignment_overrides][]
        description: List of overrides for the assignment
      - in: query
        name: assignment[automatic_peer_reviews]
        description: Whether peer reviews will be assigned automatically by Canvas
          or ifnteachers must manually assign peer reviews
      - in: query
        name: assignment[description]
        description: The assignment&#39;s description, supports HTML
      - in: query
        name: assignment[due_at]
        description: The day/time the assignment is due
      - in: query
        name: assignment[external_tool_tag_attributes]
        description: 'Hash of attributes if submission_types is [u201cexternal_toolu201d]
          Example:nnexternal_tool_tag_attributes: {n  %r/ url to the external tooln  url:
          &quot;http://instructure'
      - in: query
        name: assignment[grade_group_students_individually]
        description: If this is a group assignment, teachers have the options to grade
          studentsnindividually
      - in: query
        name: assignment[grading_standard_id]
        description: The grading standard id to set for the course
      - in: query
        name: assignment[grading_type]
        description: The strategy used for grading the assignment
      - in: query
        name: assignment[group_category_id]
        description: If present, the assignment will become a group assignment assigned
          to thengroup
      - in: query
        name: assignment[integration_data]
        description: Data related to third party integrations, JSON string required
      - in: query
        name: assignment[integration_id]
        description: Unique ID from third party integrations
      - in: query
        name: assignment[lock_at]
        description: The day/time the assignment is locked after
      - in: query
        name: assignment[muted]
        description: Whether this assignment is muted
      - in: query
        name: assignment[name]
        description: The assignment name
      - in: query
        name: assignment[notify_of_update]
        description: If true, Canvas will send a notification to students in the class
          notifyingnthem that the content has changed
      - in: query
        name: assignment[only_visible_to_overrides]
        description: Whether this assignment is only visible to overrides (Only useful
          ifn&#39;differentiated assignments&#39; account setting is on)
      - in: query
        name: assignment[peer_reviews]
        description: If submission_types does not include external_tool,discussion_topic,nonline_quiz,
          or on_paper, determines whether or not peer reviews will benturned on for
          the assignment
      - in: query
        name: assignment[points_possible]
        description: The maximum points possible on the assignment
      - in: query
        name: assignment[position]
        description: The position of this assignment in the group when displaying
          assignmentnlists
      - in: query
        name: assignment[published]
        description: Whether this assignment is published
      - in: query
        name: assignment[submission_types][]
        description: List of supported submission types for the assignment
      - in: query
        name: assignment[turnitin_enabled]
        description: Only applies when the Turnitin plugin is enabled for a course
          and thensubmission_types array includes u201conline_uploadu201d
      - in: query
        name: assignment[turnitin_settings]
        description: Settings to send along to turnitin
      - in: query
        name: assignment[unlock_at]
        description: The day/time the assignment is unlocked
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
  /courses/{course_id}/assignments/assignment_id/gradeable_students:
    get:
      summary: List gradeable students
      description: List gradeable students.
      operationId: list-gradeable-students
      x-api-path-slug: coursescourse-idassignmentsassignment-idgradeable-students-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Gradeable
      - Students
  /courses/{course_id}/assignments/assignment_id/moderated_students:
    get:
      summary: List students selected for moderation
      description: List students selected for moderation.
      operationId: list-students-selected-for-moderation
      x-api-path-slug: coursescourse-idassignmentsassignment-idmoderated-students-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Moderated
      - Students
    post:
      summary: Select students for moderation
      description: Select students for moderation.
      operationId: select-students-for-moderation
      x-api-path-slug: coursescourse-idassignmentsassignment-idmoderated-students-post
      parameters:
      - in: query
        name: student_ids[]
        description: user ids for students to select for moderation
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Moderated
      - Students
  /courses/{course_id}/assignments/assignment_id/overrides:
    get:
      summary: List assignment overrides
      description: List assignment overrides.
      operationId: list-assignment-overrides
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverrides-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
    post:
      summary: Create an assignment override
      description: Create an assignment override.
      operationId: create-an-assignment-override
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverrides-post
      parameters:
      - in: query
        name: assignment_override[course_section_id]
        description: The ID of the override&#39;s target section
      - in: query
        name: assignment_override[due_at]
        description: The day/time the overridden assignment is due
      - in: query
        name: assignment_override[group_id]
        description: The ID of the override&#39;s target group
      - in: query
        name: assignment_override[lock_at]
        description: The day/time the overridden assignment becomes locked
      - in: query
        name: assignment_override[student_ids][]
        description: The IDs of the override&#39;s target students
      - in: query
        name: assignment_override[title]
        description: The title of the adhoc assignment override
      - in: query
        name: assignment_override[unlock_at]
        description: The day/time the overridden assignment becomes unlocked
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
  /courses/{course_id}/assignments/assignment_id/overrides/{id}:
    delete:
      summary: Delete an assignment override
      description: Delete an assignment override.
      operationId: delete-an-assignment-override
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverridesid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
      - Id
    get:
      summary: Get a single assignment override
      description: Get a single assignment override.
      operationId: get-a-single-assignment-override
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverridesid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
      - Id
    put:
      summary: Update an assignment override
      description: Update an assignment override.
      operationId: update-an-assignment-override
      x-api-path-slug: coursescourse-idassignmentsassignment-idoverridesid-put
      parameters:
      - in: query
        name: assignment_override[due_at]
        description: The day/time the overridden assignment is due
      - in: query
        name: assignment_override[lock_at]
        description: The day/time the overridden assignment becomes locked
      - in: query
        name: assignment_override[student_ids][]
        description: The IDs of the override&#39;s target students
      - in: query
        name: assignment_override[title]
        description: The title of an adhoc assignment override
      - in: query
        name: assignment_override[unlock_at]
        description: The day/time the overridden assignment becomes unlocked
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Overrides
      - Id
  /courses/{course_id}/assignments/assignment_id/peer_reviews:
    get:
      summary: Get all Peer Reviews
      description: Get all peer reviews.
      operationId: get-all-peer-reviews
      x-api-path-slug: coursescourse-idassignmentsassignment-idpeer-reviews-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the peer review
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Peer
      - Reviews
  /courses/{course_id}/assignments/assignment_id/provisional_grades/publish:
    post:
      summary: Publish provisional grades for an assignment
      description: Publish provisional grades for an assignment.
      operationId: publish-provisional-grades-for-an-assignment
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradespublish-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Publish
  /courses/{course_id}/assignments/assignment_id/provisional_grades/status:
    get:
      summary: Show provisional grade status for a student
      description: Show provisional grade status for a student.
      operationId: show-provisional-grade-status-for-a-student
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradesstatus-get
      parameters:
      - in: query
        name: student_id
        description: The id of the student to show the status for
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Status
  /courses/{course_id}/assignments/assignment_id/provisional_grades/{provisional_grade_id}/copy_to_final_mark:
    post:
      summary: Copy provisional grade
      description: Copy provisional grade.
      operationId: copy-provisional-grade
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idcopy-to-final-mark-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Provisional
      - Grade
      - Id
      - Copy
      - To
      - Final
      - Mark
  /courses/{course_id}/assignments/assignment_id/provisional_grades/{provisional_grade_id}/select:
    put:
      summary: Select provisional grade
      description: Select provisional grade.
      operationId: select-provisional-grade
      x-api-path-slug: coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idselect-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Provisional
      - Grades
      - Provisional
      - Grade
      - Id
      - Select
  /courses/{course_id}/assignments/assignment_id/submissions:
    get:
      summary: List assignment submissions
      description: List assignment submissions.
      operationId: list-assignment-submissions
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissions-get
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
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
    post:
      summary: Submit an assignment
      description: Submit an assignment.
      operationId: submit-an-assignment
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissions-post
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
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
  /courses/{course_id}/assignments/assignment_id/submissions/update_grades:
    post:
      summary: Grade or comment on multiple submissions
      description: Grade or comment on multiple submissions.
      operationId: grade-or-comment-on-multiple-submissions
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsupdate-grades-post
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
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Update
      - Grades
  /courses/{course_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews:
    delete:
      summary: Create Peer Review
      description: Create peer review.
      operationId: create-peer-review
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete
      parameters:
      - in: query
        name: user_id
        description: user_id to delete as reviewer on this assignment
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
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
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the peer review
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
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
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post
      parameters:
      - in: query
        name: user_id
        description: user_id to assign as reviewer on this assignment
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - Submission
      - Id
      - Peer
      - Reviews
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}:
    get:
      summary: Get a single submission
      description: Get a single submission.
      operationId: get-a-single-submission
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-id-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the group
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
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
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-id-put
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
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}/comments/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idcommentsfiles-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Comments
      - Files
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Files
  /courses/{course_id}/assignments/assignment_id/submissions/{user_id}/read:
    delete:
      summary: Mark submission as unread
      description: Mark submission as unread.
      operationId: mark-submission-as-unread
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idread-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
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
      x-api-path-slug: coursescourse-idassignmentsassignment-idsubmissionsuser-idread-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
      - User
      - Id
      - Read
  /courses/{course_id}/assignments/id:
    delete:
      summary: Delete an assignment
      description: Delete an assignment.
      operationId: delete-an-assignment
      x-api-path-slug: coursescourse-idassignmentsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Id
    get:
      summary: Get a single assignment
      description: Get a single assignment.
      operationId: get-a-single-assignment
      x-api-path-slug: coursescourse-idassignmentsid-get
      parameters:
      - in: query
        name: all_dates
        description: All dates associated with the assignment, if applicable
      - in: query
        name: include[]
        description: Associations to include with the assignment
      - in: query
        name: needs_grading_count_by_section
        description: Split up u201cneeds_grading_countu201d by sections into thenu201cneeds_grading_count_by_sectionu201d
          key, defaults to false
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides to the assignment, defaults to true
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Id
    put:
      summary: Edit an assignment
      description: Edit an assignment.
      operationId: edit-an-assignment
      x-api-path-slug: coursescourse-idassignmentsid-put
      parameters:
      - in: query
        name: assignment[allowed_extensions][]
        description: 'Allowed extensions if submission_types includes u201conline_uploadu201dnnExample:nnallowed_extensions:
          [&quot;docx&quot;,&quot;ppt&quot;]'
      - in: query
        name: assignment[assignment_group_id]
        description: The assignment group id to put the assignment in
      - in: query
        name: assignment[assignment_overrides][]
        description: List of overrides for the assignment
      - in: query
        name: assignment[automatic_peer_reviews]
        description: Whether peer reviews will be assigned automatically by Canvas
          or ifnteachers must manually assign peer reviews
      - in: query
        name: assignment[description]
        description: The assignment&#39;s description, supports HTML
      - in: query
        name: assignment[due_at]
        description: The day/time the assignment is due
      - in: query
        name: assignment[external_tool_tag_attributes]
        description: 'Hash of attributes if submission_types is [u201cexternal_toolu201d]
          Example:nnexternal_tool_tag_attributes: {n  %r/ url to the external tooln  url:
          &quot;http://instructure'
      - in: query
        name: assignment[grade_group_students_individually]
        description: If this is a group assignment, teachers have the options to grade
          studentsnindividually
      - in: query
        name: assignment[grading_standard_id]
        description: The grading standard id to set for the course
      - in: query
        name: assignment[grading_type]
        description: The strategy used for grading the assignment
      - in: query
        name: assignment[group_category_id]
        description: If present, the assignment will become a group assignment assigned
          to thengroup
      - in: query
        name: assignment[integration_data]
        description: Data related to third party integrations, JSON string required
      - in: query
        name: assignment[integration_id]
        description: Unique ID from third party integrations
      - in: query
        name: assignment[lock_at]
        description: The day/time the assignment is locked after
      - in: query
        name: assignment[muted]
        description: Whether this assignment is muted
      - in: query
        name: assignment[name]
        description: The assignment name
      - in: query
        name: assignment[notify_of_update]
        description: If true, Canvas will send a notification to students in the class
          notifyingnthem that the content has changed
      - in: query
        name: assignment[only_visible_to_overrides]
        description: Whether this assignment is only visible to overrides (Only useful
          ifn&#39;differentiated assignments&#39; account setting is on)
      - in: query
        name: assignment[peer_reviews]
        description: If submission_types does not include external_tool,discussion_topic,nonline_quiz,
          or on_paper, determines whether or not peer reviews will benturned on for
          the assignment
      - in: query
        name: assignment[points_possible]
        description: The maximum points possible on the assignment
      - in: query
        name: assignment[position]
        description: The position of this assignment in the group when displaying
          assignmentnlists
      - in: query
        name: assignment[published]
        description: Whether this assignment is published
      - in: query
        name: assignment[submission_types][]
        description: List of supported submission types for the assignment
      - in: query
        name: assignment[turnitin_enabled]
        description: Only applies when the Turnitin plugin is enabled for a course
          and thensubmission_types array includes u201conline_uploadu201d
      - in: query
        name: assignment[turnitin_settings]
        description: Settings to send along to turnitin
      - in: query
        name: assignment[unlock_at]
        description: The day/time the assignment is unlocked
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignments
      - Id
  /courses/{course_id}/assignment_groups:
    get:
      summary: List assignment groups
      description: List assignment groups.
      operationId: list-assignment-groups
      x-api-path-slug: coursescourse-idassignment-groups-get
      parameters:
      - in: query
        name: grading_period_id
        description: The id of the grading period in which assignment groups are being
          requestedn(Requires the Multiple Grading Periods feature turned on
      - in: query
        name: include[]
        description: Associations to include with the group
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides for each assignment, defaults to true
      - in: query
        name: scope_assignments_to_student
        description: If true, all assignments returned will apply to the current user
          in thenspecified grading period
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
    post:
      summary: Create an Assignment Group
      description: Create an assignment group.
      operationId: create-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groups-post
      parameters:
      - in: query
        name: group_weight
        description: The percent of the total grade that this assignment group represents
      - in: query
        name: name
        description: The assignment group&#39;s name
      - in: query
        name: position
        description: The position of this assignment group in relation to the other
          assignmentngroups
      - in: query
        name: rules
        description: The grading rules that are applied within this assignment group
          See thenAssignment Group object definition for format
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
  /courses/{course_id}/assignment_groups/assignment_group_id:
    delete:
      summary: Destroy an Assignment Group
      description: Destroy an assignment group.
      operationId: destroy-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groupsassignment-group-id-delete
      parameters:
      - in: query
        name: move_assignments_to
        description: The ID of an active Assignment Group to which the assignments
          that arencurrently assigned to the destroyed Assignment Group will be assigned
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
      - Assignment
      - Group
      - Id
    get:
      summary: Get an Assignment Group
      description: Get an assignment group.
      operationId: get-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groupsassignment-group-id-get
      parameters:
      - in: query
        name: grading_period_id
        description: The id of the grading period in which assignment groups are being
          requestedn(Requires the Multiple Grading Periods account feature turned
          on)
      - in: query
        name: include[]
        description: Associations to include with the group
      - in: query
        name: override_assignment_dates
        description: Apply assignment overrides for each assignment, defaults to true
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
      - Assignment
      - Group
      - Id
    put:
      summary: Edit an Assignment Group
      description: Edit an assignment group.
      operationId: edit-an-assignment-group
      x-api-path-slug: coursescourse-idassignment-groupsassignment-group-id-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Assignment
      - Groups
      - Assignment
      - Group
      - Id
  /courses/{course_id}/conferences:
    get:
      summary: List conferences
      description: List conferences.
      operationId: list-conferences
      x-api-path-slug: coursescourse-idconferences-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Conferences
  /courses/{course_id}/content_exports:
    get:
      summary: List content exports
      description: List content exports.
      operationId: list-content-exports
      x-api-path-slug: coursescourse-idcontent-exports-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Exports
    post:
      summary: Export content
      description: Export content.
      operationId: export-content
      x-api-path-slug: coursescourse-idcontent-exports-post
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
      - Courses
      - Course
      - Id
      - Content
      - Exports
  /courses/{course_id}/content_exports/id:
    get:
      summary: Show content export
      description: Show content export.
      operationId: show-content-export
      x-api-path-slug: coursescourse-idcontent-exportsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Exports
      - Id
  /courses/{course_id}/content_licenses:
    get:
      summary: List licenses
      description: List licenses.
      operationId: list-licenses
      x-api-path-slug: coursescourse-idcontent-licenses-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Licenses
  /courses/{course_id}/content_migrations:
    get:
      summary: List content migrations
      description: List content migrations.
      operationId: list-content-migrations
      x-api-path-slug: coursescourse-idcontent-migrations-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Migrations
    post:
      summary: Create a content migration
      description: Create a content migration.
      operationId: create-a-content-migration
      x-api-path-slug: coursescourse-idcontent-migrations-post
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
      - Courses
      - Course
      - Id
      - Content
      - Migrations
  /courses/{course_id}/content_migrations/content_migration_id/migration_issues:
    get:
      summary: List migration issues
      description: List migration issues.
      operationId: list-migration-issues
      x-api-path-slug: coursescourse-idcontent-migrationscontent-migration-idmigration-issues-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
  /courses/{course_id}/content_migrations/content_migration_id/migration_issues/{id}:
    get:
      summary: Get a migration issue
      description: Get a migration issue.
      operationId: get-a-migration-issue
      x-api-path-slug: coursescourse-idcontent-migrationscontent-migration-idmigration-issuesid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
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
      x-api-path-slug: coursescourse-idcontent-migrationscontent-migration-idmigration-issuesid-put
      parameters:
      - in: query
        name: workflow_state
        description: Set the workflow_state of the issue
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
      - Id
  /courses/{course_id}/content_migrations/id:
    get:
      summary: Get a content migration
      description: Get a content migration.
      operationId: get-a-content-migration
      x-api-path-slug: coursescourse-idcontent-migrationsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Migrations
      - Id
    put:
      summary: Update a content migration
      description: Update a content migration.
      operationId: update-a-content-migration
      x-api-path-slug: coursescourse-idcontent-migrationsid-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Migrations
      - Id
  /courses/{course_id}/content_migrations/migrators:
    get:
      summary: List Migration Systems
      description: List migration systems.
      operationId: list-migration-systems
      x-api-path-slug: coursescourse-idcontent-migrationsmigrators-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Content
      - Migrations
      - Migrators
  /courses/{course_id}/course_copy:
    post:
      summary: Copy course content
      description: Copy course content.
      operationId: copy-course-content
      x-api-path-slug: coursescourse-idcourse-copy-post
      parameters:
      - in: query
        name: except[]
        description: A list of the course content types to exclude, all areas not
          listed will bencopied
      - in: query
        name: only[]
        description: A list of the course content types to copy, all areas not listed
          will notnbe copied
      - in: query
        name: source_course
        description: ID or SIS-ID of the course to copy the content from
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Course
      - Copy
  /courses/{course_id}/course_copy/id:
    get:
      summary: Get course copy status
      description: Get course copy status.
      operationId: get-course-copy-status
      x-api-path-slug: coursescourse-idcourse-copyid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Course
      - Copy
      - Id
  /courses/{course_id}/custom_gradebook_columns:
    get:
      summary: List custom gradebook columns
      description: List custom gradebook columns.
      operationId: list-custom-gradebook-columns
      x-api-path-slug: coursescourse-idcustom-gradebook-columns-get
      parameters:
      - in: query
        name: include_hidden
        description: Include hidden parameters (defaults to false)
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Custom
      - Gradebook
      - Columns
    post:
      summary: Create a custom gradebook column
      description: Create a custom gradebook column.
      operationId: create-a-custom-gradebook-column
      x-api-path-slug: coursescourse-idcustom-gradebook-columns-post
      parameters:
      - in: query
        name: column[hidden]
        description: Hidden columns are not displayed in the gradebook
      - in: query
        name: column[position]
        description: The position of the column relative to other custom columns
      - in: query
        name: column[teacher_notes]
        description: Set this if the column is created by a teacher
      - in: query
        name: column[title]
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Custom
      - Gradebook
      - Columns
  /courses/{course_id}/custom_gradebook_columns/id:
    delete:
      summary: Delete a custom gradebook column
      description: Delete a custom gradebook column.
      operationId: delete-a-custom-gradebook-column
      x-api-path-slug: coursescourse-idcustom-gradebook-columnsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Custom
      - Gradebook
      - Columns
      - Id
    put:
      summary: Update a custom gradebook column
      description: Update a custom gradebook column.
      operationId: update-a-custom-gradebook-column
      x-api-path-slug: coursescourse-idcustom-gradebook-columnsid-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Custom
      - Gradebook
      - Columns
      - Id
  /courses/{course_id}/custom_gradebook_columns/id/data:
    get:
      summary: List entries for a column
      description: List entries for a column.
      operationId: list-entries-for-a-column
      x-api-path-slug: coursescourse-idcustom-gradebook-columnsiddata-get
      parameters:
      - in: query
        name: include_hidden
        description: If true, hidden columns will be included in the result
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Custom
      - Gradebook
      - Columns
      - Id
      - Data
  /courses/{course_id}/custom_gradebook_columns/id/data/{user_id}:
    put:
      summary: Update column data
      description: Update column data.
      operationId: update-column-data
      x-api-path-slug: coursescourse-idcustom-gradebook-columnsiddatauser-id-put
      parameters:
      - in: query
        name: column_data[content]
        description: Column content
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Custom
      - Gradebook
      - Columns
      - Id
      - Data
      - User
      - Id
  /courses/{course_id}/custom_gradebook_columns/reorder:
    post:
      summary: Reorder custom columns
      description: Reorder custom columns.
      operationId: reorder-custom-columns
      x-api-path-slug: coursescourse-idcustom-gradebook-columnsreorder-post
      parameters:
      - in: query
        name: order[]
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Custom
      - Gradebook
      - Columns
      - Reorder
  /courses/{course_id}/discussion_topics:
    get:
      summary: List discussion topics
      description: List discussion topics.
      operationId: list-discussion-topics
      x-api-path-slug: coursescourse-iddiscussion-topics-get
      parameters:
      - in: query
        name: only_announcements
        description: Return announcements instead of discussion topics
      - in: query
        name: order_by
        description: Determines the order of the discussion topic list
      - in: query
        name: scope
        description: Only return discussion topics in the given state(s)
      - in: query
        name: search_term
        description: The partial title of the discussion topics to match and return
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
    post:
      summary: Create a new discussion topic
      description: Create a new discussion topic.
      operationId: create-a-new-discussion-topic
      x-api-path-slug: coursescourse-iddiscussion-topics-post
      parameters:
      - in: query
        name: allow_rating
        description: If true, users will be allowed to rate entries
      - in: query
        name: assignment
        description: To create an assignment discussion, pass the assignment parameters
          as ansub-object
      - in: query
        name: attachment
        description: A multipart/form-data form-field-style attachment
      - in: query
        name: delayed_post_at
        description: If a timestamp is given, the topic will not be published until
          that time
      - in: query
        name: discussion_type
        description: The type of discussion
      - in: query
        name: group_category_id
        description: If present, the topic will become a group discussion assigned
          to the group
      - in: query
        name: is_announcement
        description: If true, this topic is an announcement
      - in: query
        name: lock_at
        description: If a timestamp is given, the topic will be scheduled to lock
          at thenprovided timestamp
      - in: query
        name: message
        description: no description
      - in: query
        name: only_graders_can_rate
        description: If true, only graders will be allowed to rate entries
      - in: query
        name: pinned
        description: If true, this topic will be listed in the u201cPinned Discussionu201d
          section
      - in: query
        name: podcast_enabled
        description: If true, the topic will have an associated podcast feed
      - in: query
        name: podcast_has_student_posts
        description: If true, the podcast will include posts from students as well
      - in: query
        name: position_after
        description: By default, discussions are sorted chronologically by creation
          date, youncan pass the id of another topic to have this one show up after
          the othernwhen they are listed
      - in: query
        name: published
        description: Whether this topic is published (true) or draft state (false)
      - in: query
        name: require_initial_post
        description: If true then a user may not respond to other replies until that
          user hasnmade an initial reply
      - in: query
        name: sort_by_rating
        description: If true, entries will be sorted by rating
      - in: query
        name: title
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
  /courses/{course_id}/discussion_topics/reorder:
    post:
      summary: Reorder pinned topics
      description: Reorder pinned topics.
      operationId: reorder-pinned-topics
      x-api-path-slug: coursescourse-iddiscussion-topicsreorder-post
      parameters:
      - in: query
        name: order[]
        description: The ids of the pinned discussion topics in the desired order
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Reorder
  /courses/{course_id}/discussion_topics/topic_id:
    delete:
      summary: Delete a topic
      description: Delete a topic.
      operationId: delete-a-topic
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-id-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
    get:
      summary: Get a single topic
      description: Get a single topic.
      operationId: get-a-single-topic
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-id-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
    put:
      summary: Update a topic
      description: Update a topic.
      operationId: update-a-topic
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-id-put
      parameters:
      - in: query
        name: allow_rating
        description: If true, users will be allowed to rate entries
      - in: query
        name: assignment
        description: To create an assignment discussion, pass the assignment parameters
          as ansub-object
      - in: query
        name: delayed_post_at
        description: If a timestamp is given, the topic will not be published until
          that time
      - in: query
        name: discussion_type
        description: The type of discussion
      - in: query
        name: group_category_id
        description: If present, the topic will become a group discussion assigned
          to the group
      - in: query
        name: is_announcement
        description: If true, this topic is an announcement
      - in: query
        name: lock_at
        description: If a timestamp is given, the topic will be scheduled to lock
          at thenprovided timestamp
      - in: query
        name: message
        description: no description
      - in: query
        name: only_graders_can_rate
        description: If true, only graders will be allowed to rate entries
      - in: query
        name: pinned
        description: If true, this topic will be listed in the u201cPinned Discussionu201d
          section
      - in: query
        name: podcast_enabled
        description: If true, the topic will have an associated podcast feed
      - in: query
        name: podcast_has_student_posts
        description: If true, the podcast will include posts from students as well
      - in: query
        name: position_after
        description: By default, discussions are sorted chronologically by creation
          date, youncan pass the id of another topic to have this one show up after
          the othernwhen they are listed
      - in: query
        name: published
        description: Whether this topic is published (true) or draft state (false)
      - in: query
        name: require_initial_post
        description: If true then a user may not respond to other replies until that
          user hasnmade an initial reply
      - in: query
        name: sort_by_rating
        description: If true, entries will be sorted by rating
      - in: query
        name: title
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
  /courses/{course_id}/discussion_topics/topic_id/entries:
    get:
      summary: List topic entries
      description: List topic entries.
      operationId: list-topic-entries
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identries-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
    post:
      summary: Post an entry
      description: Post an entry.
      operationId: post-an-entry
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identries-post
      parameters:
      - in: query
        name: attachment
        description: a multipart/form-data form-field-style attachment
      - in: query
        name: message
        description: The body of the entry
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
  /courses/{course_id}/discussion_topics/topic_id/entries/{entry_id}/rating:
    post:
      summary: Rate entry
      description: Rate entry.
      operationId: rate-entry
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identriesentry-idrating-post
      parameters:
      - in: query
        name: rating
        description: A rating to set on this entry
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Rating
  /courses/{course_id}/discussion_topics/topic_id/entries/{entry_id}/read:
    delete:
      summary: Mark entry as unread
      description: Mark entry as unread.
      operationId: mark-entry-as-unread
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identriesentry-idread-delete
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set the entry&#39;s forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Read
    put:
      summary: Mark entry as read
      description: Mark entry as read.
      operationId: mark-entry-as-read
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identriesentry-idread-put
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set the entry&#39;s forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Read
  /courses/{course_id}/discussion_topics/topic_id/entries/{entry_id}/replies:
    get:
      summary: List entry replies
      description: List entry replies.
      operationId: list-entry-replies
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identriesentry-idreplies-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Replies
    post:
      summary: Post a reply
      description: Post a reply.
      operationId: post-a-reply
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identriesentry-idreplies-post
      parameters:
      - in: query
        name: attachment
        description: a multipart/form-data form-field-style attachment
      - in: query
        name: message
        description: The body of the entry
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Replies
  /courses/{course_id}/discussion_topics/topic_id/entries/{id}:
    delete:
      summary: Delete an entry
      description: Delete an entry.
      operationId: delete-an-entry
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identriesid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Id
    put:
      summary: Update an entry
      description: Update an entry.
      operationId: update-an-entry
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identriesid-put
      parameters:
      - in: query
        name: message
        description: The updated body of the entry
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Id
  /courses/{course_id}/discussion_topics/topic_id/entry_list:
    get:
      summary: List entries
      description: List entries.
      operationId: list-entries
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identry-list-get
      parameters:
      - in: query
        name: ids[]
        description: A list of entry ids to retrieve
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entry
      - List
  /courses/{course_id}/discussion_topics/topic_id/read:
    delete:
      summary: Mark topic as unread
      description: Mark topic as unread.
      operationId: mark-topic-as-unread
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-idread-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
    put:
      summary: Mark topic as read
      description: Mark topic as read.
      operationId: mark-topic-as-read
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-idread-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
  /courses/{course_id}/discussion_topics/topic_id/read_all:
    delete:
      summary: Mark all entries as unread
      description: Mark all entries as unread.
      operationId: mark-all-entries-as-unread
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-idread-all-delete
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set all of the entries&#39; forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
    put:
      summary: Mark all entries as read
      description: Mark all entries as read.
      operationId: mark-all-entries-as-read
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-idread-all-put
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set all of the entries&#39; forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
  /courses/{course_id}/discussion_topics/topic_id/subscribed:
    delete:
      summary: Unsubscribe from a topic
      description: Unsubscribe from a topic.
      operationId: unsubscribe-from-a-topic
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-idsubscribed-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Subscribed
    put:
      summary: Subscribe to a topic
      description: Subscribe to a topic.
      operationId: subscribe-to-a-topic
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-idsubscribed-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Subscribed
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