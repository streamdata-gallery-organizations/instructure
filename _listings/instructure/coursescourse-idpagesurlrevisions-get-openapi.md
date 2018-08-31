---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API List revisions
  description: List revisions.
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
  /appointment_groups:
    get:
      summary: List appointment groups
      description: List appointment groups.
      operationId: list-appointment-groups
      x-api-path-slug: appointment-groups-get
      parameters:
      - in: query
        name: context_codes[]
        description: Array of context codes used to limit returned results
      - in: query
        name: include[]
        description: Array of additional information to include
      - in: query
        name: include_past_appointments
        description: Defaults to false
      - in: query
        name: scope
        description: 'Defaults to u201creservableu201dnn        n        n          Allowed
          values: reservable, manageable'
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
    post:
      summary: Create an appointment group
      description: Create an appointment group.
      operationId: create-an-appointment-group
      x-api-path-slug: appointment-groups-post
      parameters:
      - in: query
        name: appointment_group[context_codes][]
        description: Array of context codes (courses, e
      - in: query
        name: appointment_group[description]
        description: Longer text description of the appointment group
      - in: query
        name: appointment_group[location_address]
        description: Location address
      - in: query
        name: appointment_group[location_name]
        description: Location name of the appointment group
      - in: query
        name: appointment_group[max_appointments_per_participant]
        description: Maximum number of time slots a user may register for
      - in: query
        name: appointment_group[min_appointments_per_participant]
        description: Minimum number of time slots a user must register for
      - in: query
        name: appointment_group[new_appointments][X][]
        description: Nested array of start time/end time pairs indicating time slots
          for thisnappointment group
      - in: query
        name: appointment_group[participants_per_appointment]
        description: Maximum number of participants that may register for each time
          slot
      - in: query
        name: appointment_group[participant_visibility]
        description: u201cprivateu201dnnparticipants cannot see who has signed up
          for a particular time slotnu201cprotectedu201dnnparticipants can see who
          has signed up
      - in: query
        name: appointment_group[publish]
        description: Indicates whether this appointment group should be published
          (i
      - in: query
        name: appointment_group[sub_context_codes][]
        description: Array of sub context codes (course sections or a single group
          category)nthis group should be linked to
      - in: query
        name: appointment_group[title]
        description: Short title for the appointment group
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
  /appointment_groups/{id}:
    delete:
      summary: Delete an appointment group
      description: Delete an appointment group.
      operationId: delete-an-appointment-group
      x-api-path-slug: appointment-groupsid-delete
      parameters:
      - in: query
        name: cancel_reason
        description: Reason for deleting/canceling the appointment group
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
    get:
      summary: Get a single appointment group
      description: Get a single appointment group.
      operationId: get-a-single-appointment-group
      x-api-path-slug: appointment-groupsid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
    put:
      summary: Update an appointment group
      description: Update an appointment group.
      operationId: update-an-appointment-group
      x-api-path-slug: appointment-groupsid-put
      parameters:
      - in: query
        name: appointment_group[context_codes][]
        description: Array of context codes (courses, e
      - in: query
        name: appointment_group[description]
        description: Longer text description of the appointment group
      - in: query
        name: appointment_group[location_address]
        description: Location address
      - in: query
        name: appointment_group[location_name]
        description: Location name of the appointment group
      - in: query
        name: appointment_group[max_appointments_per_participant]
        description: Maximum number of time slots a user may register for
      - in: query
        name: appointment_group[min_appointments_per_participant]
        description: Minimum number of time slots a user must register for
      - in: query
        name: appointment_group[new_appointments][X][]
        description: Nested array of start time/end time pairs indicating time slots
          for thisnappointment group
      - in: query
        name: appointment_group[participants_per_appointment]
        description: Maximum number of participants that may register for each time
          slot
      - in: query
        name: appointment_group[participant_visibility]
        description: u201cprivateu201dnnparticipants cannot see who has signed up
          for a particular time slotnu201cprotectedu201dnnparticipants can see who
          has signed up
      - in: query
        name: appointment_group[publish]
        description: Indicates whether this appointment group should be published
          (i
      - in: query
        name: appointment_group[sub_context_codes][]
        description: Array of sub context codes (course sections or a single group
          category)nthis group should be linked to
      - in: query
        name: appointment_group[title]
        description: Short title for the appointment group
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
  /appointment_groups/{id}/groups:
    get:
      summary: List student group participants
      description: List student group participants.
      operationId: list-student-group-participants
      x-api-path-slug: appointment-groupsidgroups-get
      parameters:
      - in: query
        name: registration_status
        description: 'Limits results to the a given participation status, defaults
          to u201callu201dnn        n        n          Allowed values: all, registered,
          registered'
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
      - Groups
  /appointment_groups/{id}/users:
    get:
      summary: List user participants
      description: List user participants.
      operationId: list-user-participants
      x-api-path-slug: appointment-groupsidusers-get
      parameters:
      - in: query
        name: registration_status
        description: 'Limits results to the a given participation status, defaults
          to u201callu201dnn        n        n          Allowed values: all, registered,
          registered'
      responses:
        200:
          description: OK
      tags:
      - Appointment
      - Groups
      - Id
      - Users
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
  /audit/grade_change/students/{student_id}:
    get:
      summary: Query by student.
      description: Query by student..
      operationId: query-by-student
      x-api-path-slug: auditgrade-changestudentsstudent-id-get
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
      - Students
      - Student
      - Id
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
    post:
      summary: Create a calendar event
      description: Create a calendar event.
      operationId: create-a-calendar-event
      x-api-path-slug: calendar-events-post
      parameters:
      - in: query
        name: calendar_event[child_event_data][X][context_code]
        description: Context code(s) corresponding to the section-level start and
          end time(s)
      - in: query
        name: calendar_event[child_event_data][X][end_at]
        description: Section-level end time(s) if this is a course event
      - in: query
        name: calendar_event[child_event_data][X][start_at]
        description: Section-level start time(s) if this is a course event
      - in: query
        name: calendar_event[context_code]
        description: Context code of the course/group/user whose calendar this event
          should benadded to
      - in: query
        name: calendar_event[description]
        description: Longer HTML description of the event
      - in: query
        name: calendar_event[duplicate][append_iterator]
        description: Defaults to false
      - in: query
        name: calendar_event[duplicate][count]
        description: Number of times to copy/duplicate the event
      - in: query
        name: calendar_event[duplicate][frequency]
        description: Defaults to u201cweeklyu201d
      - in: query
        name: calendar_event[duplicate][interval]
        description: Defaults to 1 if duplicate `count` is set
      - in: query
        name: calendar_event[end_at]
        description: End date/time of the event
      - in: query
        name: calendar_event[location_address]
        description: Location address
      - in: query
        name: calendar_event[location_name]
        description: Location name of the event
      - in: query
        name: calendar_event[start_at]
        description: Start date/time of the event
      - in: query
        name: calendar_event[time_zone_edited]
        description: Time zone of the user editing the event
      - in: query
        name: calendar_event[title]
        description: Short title for the calendar event
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
  /calendar_events/{id}:
    delete:
      summary: Delete a calendar event
      description: Delete a calendar event.
      operationId: delete-a-calendar-event
      x-api-path-slug: calendar-eventsid-delete
      parameters:
      - in: query
        name: cancel_reason
        description: Reason for deleting/canceling the event
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
    get:
      summary: Get a single calendar event or assignment
      description: Get a single calendar event or assignment.
      operationId: get-a-single-calendar-event-or-assignment
      x-api-path-slug: calendar-eventsid-get
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
    put:
      summary: Update a calendar event
      description: Update a calendar event.
      operationId: update-a-calendar-event
      x-api-path-slug: calendar-eventsid-put
      parameters:
      - in: query
        name: calendar_event[child_event_data][X][context_code]
        description: Context code(s) corresponding to the section-level start and
          end time(s)
      - in: query
        name: calendar_event[child_event_data][X][end_at]
        description: Section-level end time(s) if this is a course event
      - in: query
        name: calendar_event[child_event_data][X][start_at]
        description: Section-level start time(s) if this is a course event
      - in: query
        name: calendar_event[context_code]
        description: Context code of the course/group/user whose calendar this event
          should benadded to
      - in: query
        name: calendar_event[description]
        description: Longer HTML description of the event
      - in: query
        name: calendar_event[end_at]
        description: End date/time of the event
      - in: query
        name: calendar_event[location_address]
        description: Location address
      - in: query
        name: calendar_event[location_name]
        description: Location name of the event
      - in: query
        name: calendar_event[start_at]
        description: Start date/time of the event
      - in: query
        name: calendar_event[time_zone_edited]
        description: Time zone of the user editing the event
      - in: query
        name: calendar_event[title]
        description: Short title for the calendar event
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
  /calendar_events/{id}/reservations:
    post:
      summary: Reserve a time slot
      description: Reserve a time slot.
      operationId: reserve-a-time-slot
      x-api-path-slug: calendar-eventsidreservations-post
      parameters:
      - in: query
        name: cancel_existing
        description: Defaults to false
      - in: query
        name: comments
        description: Comments to associate with this reservation
      - in: query
        name: participant_id
        description: User or group id for whom you are making the reservation (depends
          on thenparticipant type)
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
      - Reservations
  /calendar_events/{id}/reservations/participant_id:
    post:
      summary: Reserve a time slot
      description: Reserve a time slot.
      operationId: reserve-a-time-slot
      x-api-path-slug: calendar-eventsidreservationsparticipant-id-post
      parameters:
      - in: query
        name: cancel_existing
        description: Defaults to false
      - in: query
        name: comments
        description: Comments to associate with this reservation
      - in: query
        name: participant_id
        description: User or group id for whom you are making the reservation (depends
          on thenparticipant type)
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
      - Reservations
      - Participant
      - Id
  /conversations:
    get:
      summary: List conversations
      description: List conversations.
      operationId: list-conversations
      x-api-path-slug: conversations-get
      parameters:
      - in: query
        name: filter[]
        description: When set, only return conversations for the specified courses,
          groups ornusers
      - in: query
        name: filter_mode
        description: 'When filter[] contains multiple filters, combine them with this
          mode,nfiltering conversations that at have at least all of the contexts
          (u201candu201d)nor at least one of the contexts (u201coru201d)nn        n        n          Allowed
          values: and, or, default or'
      - in: query
        name: include_all_conversation_ids
        description: Default is false
      - in: query
        name: interleave_submissions
        description: (Obsolete) Submissions are no longer linked to conversations
      - in: query
        name: scope
        description: When set, only return conversations of the specified type
      responses:
        200:
          description: OK
      tags:
      - Conversations
    post:
      summary: Create a conversation
      description: Create a conversation.
      operationId: create-a-conversation
      x-api-path-slug: conversations-post
      parameters:
      - in: query
        name: attachment_ids[]
        description: An array of attachments ids
      - in: query
        name: body
        description: The message to be sent
      - in: query
        name: context_code
        description: The course or group that is the context for this conversation
      - in: query
        name: filter[]
        description: Used when generating u201cvisibleu201d in the API response
      - in: query
        name: filter_mode
        description: Used when generating u201cvisibleu201d in the API response
      - in: query
        name: group_conversation
        description: Defaults to false
      - in: query
        name: media_comment_id
        description: Media comment id of an audio of video file to be associated with
          thisnmessage
      - in: query
        name: media_comment_type
        description: 'Type of the associated media filenn        n        n          Allowed
          values: audio, video'
      - in: query
        name: mode
        description: Determines whether the messages will be created/sent synchronously
          ornasynchronously
      - in: query
        name: recipients[]
        description: An array of recipient ids
      - in: query
        name: scope
        description: Used when generating u201cvisibleu201d in the API response
      - in: query
        name: subject
        description: The subject of the conversation
      - in: query
        name: user_note
        description: Will add a faculty journal entry for each recipient as long as
          the usernmaking the api call has permission, the recipient is a student
          and facultynjournals are enabled in the account
      responses:
        200:
          description: OK
      tags:
      - Conversations
    put:
      summary: Batch update conversations
      description: Batch update conversations.
      operationId: batch-update-conversations
      x-api-path-slug: conversations-put
      parameters:
      - in: query
        name: conversation_ids[]
        description: List of conversations to update
      - in: query
        name: event
        description: The action to take on each conversation
      responses:
        200:
          description: OK
      tags:
      - Conversations
  /conversations/batches:
    get:
      summary: Get running batches
      description: Get running batches.
      operationId: get-running-batches
      x-api-path-slug: conversationsbatches-get
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Batches
  /conversations/find_recipients:
    get:
      summary: Find recipients
      description: Find recipients.
      operationId: find-recipients
      x-api-path-slug: conversationsfind-recipients-get
      parameters:
      - in: query
        name: context
        description: Limit the search to a particular course/group (e
      - in: query
        name: exclude[]
        description: Array of ids to exclude from the search
      - in: query
        name: from_conversation_id
        description: When searching by user_id, only users that could be normally
          messaged bynthis user will be returned
      - in: query
        name: permissions[]
        description: Array of permission strings to be checked for each matched context
          (e
      - in: query
        name: search
        description: Search terms used for matching users/courses/groups (e
      - in: query
        name: type
        description: Limit the search just to users or contexts (groups/courses)
      - in: query
        name: user_id
        description: Search for a specific user id
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Find
      - Recipients
  /conversations/mark_all_as_read:
    post:
      summary: Mark all as read
      description: Mark all as read.
      operationId: mark-all-as-read
      x-api-path-slug: conversationsmark-all-as-read-post
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Mark
      - ""
      - As
      - Read
  /conversations/unread_count:
    get:
      summary: Unread count
      description: Unread count.
      operationId: unread-count
      x-api-path-slug: conversationsunread-count-get
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Unread
      - Count
  /conversations/{id}:
    delete:
      summary: Delete a conversation
      description: Delete a conversation.
      operationId: delete-a-conversation
      x-api-path-slug: conversationsid-delete
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Id
    get:
      summary: Get a single conversation
      description: Get a single conversation.
      operationId: get-a-single-conversation
      x-api-path-slug: conversationsid-get
      parameters:
      - in: query
        name: auto_mark_as_read
        description: Default true
      - in: query
        name: filter[]
        description: Used when generating u201cvisibleu201d in the API response
      - in: query
        name: filter_mode
        description: Used when generating u201cvisibleu201d in the API response
      - in: query
        name: interleave_submissions
        description: (Obsolete) Submissions are no longer linked to conversations
      - in: query
        name: scope
        description: Used when generating u201cvisibleu201d in the API response
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Id
    put:
      summary: Edit a conversation
      description: Edit a conversation.
      operationId: edit-a-conversation
      x-api-path-slug: conversationsid-put
      parameters:
      - in: query
        name: conversation[starred]
        description: Toggle the starred state of the current user&#39;s view of thenconversation
      - in: query
        name: conversation[subject]
        description: Change the subject of this conversation
      - in: query
        name: conversation[subscribed]
        description: Toggle the current user&#39;s subscription to the conversation
          (only validnfor group conversations)
      - in: query
        name: conversation[workflow_state]
        description: 'Change the state of this conversationnn        n        n          Allowed
          values: read, unread, archived'
      - in: query
        name: filter[]
        description: Used when generating u201cvisibleu201d in the API response
      - in: query
        name: filter_mode
        description: Used when generating u201cvisibleu201d in the API response
      - in: query
        name: scope
        description: Used when generating u201cvisibleu201d in the API response
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Id
  /conversations/{id}/add_message:
    post:
      summary: Add a message
      description: Add a message.
      operationId: add-a-message
      x-api-path-slug: conversationsidadd-message-post
      parameters:
      - in: query
        name: attachment_ids[]
        description: An array of attachments ids
      - in: query
        name: body
        description: The message to be sent
      - in: query
        name: included_messages[]
        description: no description
      - in: query
        name: media_comment_id
        description: Media comment id of an audio of video file to be associated with
          thisnmessage
      - in: query
        name: media_comment_type
        description: Type of the associated media file
      - in: query
        name: recipients[]
        description: no description
      - in: query
        name: user_note
        description: Will add a faculty journal entry for each recipient as long as
          the usernmaking the api call has permission, the recipient is a student
          and facultynjournals are enabled in the account
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Id
      - Add
      - Message
  /conversations/{id}/add_recipients:
    post:
      summary: Add recipients
      description: Add recipients.
      operationId: add-recipients
      x-api-path-slug: conversationsidadd-recipients-post
      parameters:
      - in: query
        name: recipients[]
        description: An array of recipient ids
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Id
      - Add
      - Recipients
  /conversations/{id}/remove_messages:
    post:
      summary: Delete a message
      description: Delete a message.
      operationId: delete-a-message
      x-api-path-slug: conversationsidremove-messages-post
      parameters:
      - in: query
        name: remove[]
        description: Array of message ids to be deleted
      responses:
        200:
          description: OK
      tags:
      - Conversations
      - Id
      - Remove
      - Messages
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
  /courses/{course_id}/discussion_topics/topic_id/view:
    get:
      summary: Get the full topic
      description: Get the full topic.
      operationId: get-the-full-topic
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-idview-get
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
      - View
  /courses/{course_id}/enrollments:
    get:
      summary: List enrollments
      description: List enrollments.
      operationId: list-enrollments
      x-api-path-slug: coursescourse-idenrollments-get
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
      - Courses
      - Course
      - Id
      - Enrollments
    post:
      summary: Enroll a user
      description: Enroll a user.
      operationId: enroll-a-user
      x-api-path-slug: coursescourse-idenrollments-post
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
      - Courses
      - Course
      - Id
      - Enrollments
  /courses/{course_id}/enrollments/id:
    delete:
      summary: Conclude or inactivate an enrollment
      description: Conclude or inactivate an enrollment.
      operationId: conclude-or-inactivate-an-enrollment
      x-api-path-slug: coursescourse-idenrollmentsid-delete
      parameters:
      - in: query
        name: task
        description: The action to take on the enrollment
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Enrollments
      - Id
  /courses/{course_id}/enrollments/id/reactivate:
    put:
      summary: Re-activate an enrollment
      description: Re-activate an enrollment.
      operationId: reactivate-an-enrollment
      x-api-path-slug: coursescourse-idenrollmentsidreactivate-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Enrollments
      - Id
      - Reactivate
  /courses/{course_id}/epub_exports/id:
    get:
      summary: Show ePub export
      description: Show epub export.
      operationId: show-epub-export
      x-api-path-slug: coursescourse-idepub-exportsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Epub
      - Exports
      - Id
  /courses/{course_id}/external_feeds:
    get:
      summary: List external feeds
      description: List external feeds.
      operationId: list-external-feeds
      x-api-path-slug: coursescourse-idexternal-feeds-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Feeds
    post:
      summary: Create an external feed
      description: Create an external feed.
      operationId: create-an-external-feed
      x-api-path-slug: coursescourse-idexternal-feeds-post
      parameters:
      - in: query
        name: header_match
        description: If given, only feed entries that contain this string in their
          title will benimported
      - in: query
        name: url
        description: The url to the external rss or atom feed
      - in: query
        name: verbosity
        description: 'Defaults to u201cfullu201dnn        n        n          Allowed
          values: full, truncate, link_only'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Feeds
  /courses/{course_id}/external_feeds/external_feed_id:
    delete:
      summary: Delete an external feed
      description: Delete an external feed.
      operationId: delete-an-external-feed
      x-api-path-slug: coursescourse-idexternal-feedsexternal-feed-id-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Feeds
      - External
      - Feed
      - Id
  /courses/{course_id}/external_tools:
    get:
      summary: List external tools
      description: List external tools.
      operationId: list-external-tools
      x-api-path-slug: coursescourse-idexternal-tools-get
      parameters:
      - in: query
        name: search_term
        description: The partial name of the tools to match and return
      - in: query
        name: selectable
        description: If true, then only tools that are meant to be selectable are
          returned
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Tools
    post:
      summary: Create an external tool
      description: Create an external tool.
      operationId: create-an-external-tool
      x-api-path-slug: coursescourse-idexternal-tools-post
      parameters:
      - in: query
        name: account_navigation[enabled]
        description: Set this to enable this feature
      - in: query
        name: account_navigation[text]
        description: The text that will show on the left-tab in the account navigation
      - in: query
        name: account_navigation[url]
        description: The url of the external tool for account navigation
      - in: query
        name: config_type
        description: Configuration can be passed in as CC xml instead of using query
          parameters
      - in: query
        name: config_url
        description: URL where the server can retrieve an XML tool configuration,
          as specifiednin the CC xml specification
      - in: query
        name: config_xml
        description: XML tool configuration, as specified in the CC xml specification
      - in: query
        name: consumer_key
        description: The consumer key for the external tool
      - in: query
        name: course_navigation[default]
        description: Whether the navigation option will show in the course by default
          or whethernthe teacher will have to explicitly enable it
      - in: query
        name: course_navigation[enabled]
        description: Set this to enable this feature
      - in: query
        name: course_navigation[text]
        description: The text that will show on the left-tab in the course navigation
      - in: query
        name: course_navigation[url]
        description: The url of the external tool for course navigation
      - in: query
        name: course_navigation[visibility]
        description: Who will see the navigation tab
      - in: query
        name: custom_fields
        description: Custom fields that will be sent to the tool consumer, specified
          as custom_fields
      - in: query
        name: description
        description: A description of the tool
      - in: query
        name: domain
        description: The domain to match links against
      - in: query
        name: editor_button[enabled]
        description: Set this to enable this feature
      - in: query
        name: editor_button[icon_url]
        description: The url of the icon to show in the WYSIWYG editor
      - in: query
        name: editor_button[selection_height]
        description: The height of the dialog the tool is launched in
      - in: query
        name: editor_button[selection_width]
        description: The width of the dialog the tool is launched in
      - in: query
        name: editor_button[url]
        description: The url of the external tool
      - in: query
        name: icon_url
        description: The url of the icon to show for this tool
      - in: query
        name: name
        description: The name of the tool
      - in: query
        name: not_selectable
        description: 'Default: false, if set to true the tool won&#39;t show up in
          the externalntool selection UI in modules and assignments'
      - in: query
        name: privacy_level
        description: What information to send to the external tool
      - in: query
        name: resource_selection[enabled]
        description: Set this to enable this feature
      - in: query
        name: resource_selection[icon_url]
        description: The url of the icon to show in the module external tool list
      - in: query
        name: resource_selection[selection_height]
        description: The height of the dialog the tool is launched in
      - in: query
        name: resource_selection[selection_width]
        description: The width of the dialog the tool is launched in
      - in: query
        name: resource_selection[url]
        description: The url of the external tool
      - in: query
        name: shared_secret
        description: The shared secret with the external tool
      - in: query
        name: text
        description: The default text to show for this tool
      - in: query
        name: url
        description: The url to match links against
      - in: query
        name: user_navigation[enabled]
        description: Set this to enable this feature
      - in: query
        name: user_navigation[text]
        description: The text that will show on the left-tab in the user navigation
      - in: query
        name: user_navigation[url]
        description: The url of the external tool for user navigation
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Tools
  /courses/{course_id}/external_tools/external_tool_id:
    delete:
      summary: Delete an external tool
      description: Delete an external tool.
      operationId: delete-an-external-tool
      x-api-path-slug: coursescourse-idexternal-toolsexternal-tool-id-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Tools
      - External
      - Tool
      - Id
    get:
      summary: Get a single external tool
      description: Get a single external tool.
      operationId: get-a-single-external-tool
      x-api-path-slug: coursescourse-idexternal-toolsexternal-tool-id-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Tools
      - External
      - Tool
      - Id
    put:
      summary: Edit an external tool
      description: Edit an external tool.
      operationId: edit-an-external-tool
      x-api-path-slug: coursescourse-idexternal-toolsexternal-tool-id-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Tools
      - External
      - Tool
      - Id
  /courses/{course_id}/external_tools/sessionless_launch:
    get:
      summary: Get a sessionless launch url for an external tool.
      description: Get a sessionless launch url for an external tool..
      operationId: get-a-sessionless-launch-url-for-an-external-tool
      x-api-path-slug: coursescourse-idexternal-toolssessionless-launch-get
      parameters:
      - in: query
        name: assignment_id
        description: The assignment id for an assignment launch
      - in: query
        name: id
        description: The external id of the tool to launch
      - in: query
        name: launch_type
        description: The type of launch to perform on the external tool
      - in: query
        name: url
        description: The LTI launch url for the external tool
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - External
      - Tools
      - Sessionless
      - Launch
  /courses/{course_id}/features:
    get:
      summary: List features
      description: List features.
      operationId: list-features
      x-api-path-slug: coursescourse-idfeatures-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
  /courses/{course_id}/features/enabled:
    get:
      summary: List enabled features
      description: List enabled features.
      operationId: list-enabled-features
      x-api-path-slug: coursescourse-idfeaturesenabled-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
      - Enabled
  /courses/{course_id}/features/flags/feature:
    delete:
      summary: Remove feature flag
      description: Remove feature flag.
      operationId: remove-feature-flag
      x-api-path-slug: coursescourse-idfeaturesflagsfeature-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
      - Flags
      - Feature
    get:
      summary: Get feature flag
      description: Get feature flag.
      operationId: get-feature-flag
      x-api-path-slug: coursescourse-idfeaturesflagsfeature-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
      - Flags
      - Feature
    put:
      summary: Set feature flag
      description: Set feature flag.
      operationId: set-feature-flag
      x-api-path-slug: coursescourse-idfeaturesflagsfeature-put
      parameters:
      - in: query
        name: locking_account_id
        description: If set, this FeatureFlag may only be modified by someone withnadministrative
          rights in the specified account
      - in: query
        name: state
        description: u201coffu201dnnThe feature is not available for the course, user,
          or account andnsub-accounts
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Features
      - Flags
      - Feature
  /courses/{course_id}/files:
    get:
      summary: List files
      description: List files.
      operationId: list-files
      x-api-path-slug: coursescourse-idfiles-get
      parameters:
      - in: query
        name: content_types[]
        description: Filter results by content-type
      - in: query
        name: include[]
        description: Array of additional information to include
      - in: query
        name: only[]
        description: Array of information to restrict to
      - in: query
        name: order
        description: The sorting order
      - in: query
        name: search_term
        description: The partial name of the files to match and return
      - in: query
        name: sort
        description: Sort results by this field
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Files
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Files
  /courses/{course_id}/files/id:
    get:
      summary: Get file
      description: Get file.
      operationId: get-file
      x-api-path-slug: coursescourse-idfilesid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Files
      - Id
  /courses/{course_id}/files/quota:
    get:
      summary: Get quota information
      description: Get quota information.
      operationId: get-quota-information
      x-api-path-slug: coursescourse-idfilesquota-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Files
      - Quota
  /courses/{course_id}/folders:
    get:
      summary: List all folders
      description: List all folders.
      operationId: list-all-folders
      x-api-path-slug: coursescourse-idfolders-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Folders
    post:
      summary: Create folder
      description: Create folder.
      operationId: create-folder
      x-api-path-slug: coursescourse-idfolders-post
      parameters:
      - in: query
        name: hidden
        description: Flag the folder as hidden
      - in: query
        name: locked
        description: Flag the folder as locked
      - in: query
        name: lock_at
        description: The datetime to lock the folder at
      - in: query
        name: name
        description: The name of the folder
      - in: query
        name: parent_folder_id
        description: The id of the folder to store the file in
      - in: query
        name: parent_folder_path
        description: The path of the folder to store the new folder in
      - in: query
        name: position
        description: Set an explicit sort position for the folder
      - in: query
        name: unlock_at
        description: The datetime to unlock the folder at
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Folders
  /courses/{course_id}/folders/by_path:
    get:
      summary: Resolve path
      description: Resolve path.
      operationId: resolve-path
      x-api-path-slug: coursescourse-idfoldersby-path-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Folders
      - By
      - Path
  /courses/{course_id}/folders/by_path/*full_path:
    get:
      summary: Resolve path
      description: Resolve path.
      operationId: resolve-path
      x-api-path-slug: coursescourse-idfoldersby-pathfull-path-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Folders
      - By
      - Path
      - '*full'
      - Path
  /courses/{course_id}/folders/id:
    get:
      summary: Get folder
      description: Get folder.
      operationId: get-folder
      x-api-path-slug: coursescourse-idfoldersid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Folders
      - Id
  /courses/{course_id}/front_page:
    get:
      summary: Show front page
      description: Show front page.
      operationId: show-front-page
      x-api-path-slug: coursescourse-idfront-page-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Front
      - Page
    put:
      summary: Update/create front page
      description: Update/create front page.
      operationId: updatecreate-front-page
      x-api-path-slug: coursescourse-idfront-page-put
      parameters:
      - in: query
        name: wiki_page[body]
        description: The content for the new page
      - in: query
        name: wiki_page[editing_roles]
        description: Which user roles are allowed to edit this page
      - in: query
        name: wiki_page[notify_of_update]
        description: Whether participants should be notified when this page changes
      - in: query
        name: wiki_page[published]
        description: Whether the page is published (true) or draft state (false)
      - in: query
        name: wiki_page[title]
        description: The title for the new page
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Front
      - Page
  /courses/{course_id}/gradebook_history/date:
    get:
      summary: Details for a given date in gradebook history for this course
      description: Details for a given date in gradebook history for this course.
      operationId: details-for-a-given-date-in-gradebook-history-for-this-course
      x-api-path-slug: coursescourse-idgradebook-historydate-get
      parameters:
      - in: query
        name: course_id
        description: The id of the contextual course for this API call
      - in: query
        name: date
        description: The date for which you would like to see detailed information
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Gradebook
      - History
      - Date
  /courses/{course_id}/gradebook_history/date/graders/{grader_id}/assignments/assignment_id/submissions:
    get:
      summary: Lists submissions
      description: Lists submissions.
      operationId: lists-submissions
      x-api-path-slug: coursescourse-idgradebook-historydategradersgrader-idassignmentsassignment-idsubmissions-get
      parameters:
      - in: query
        name: assignment_id
        description: The ID of the assignment for which you want to see submissions
      - in: query
        name: course_id
        description: The id of the contextual course for this API call
      - in: query
        name: date
        description: The date for which you would like to see submissions
      - in: query
        name: grader_id
        description: The ID of the grader for which you want to see submissions
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Gradebook
      - History
      - Date
      - Graders
      - Grader
      - Id
      - Assignments
      - Assignment
      - Id
      - Submissions
  /courses/{course_id}/gradebook_history/days:
    get:
      summary: Days in gradebook history for this course
      description: Days in gradebook history for this course.
      operationId: days-in-gradebook-history-for-this-course
      x-api-path-slug: coursescourse-idgradebook-historydays-get
      parameters:
      - in: query
        name: course_id
        description: The id of the contextual course for this API call
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Gradebook
      - History
      - Days
  /courses/{course_id}/gradebook_history/feed:
    get:
      summary: List uncollated submission versions
      description: List uncollated submission versions.
      operationId: list-uncollated-submission-versions
      x-api-path-slug: coursescourse-idgradebook-historyfeed-get
      parameters:
      - in: query
        name: ascending
        description: Returns submission versions in ascending date order (oldest first)
      - in: query
        name: assignment_id
        description: The ID of the assignment for which you want to see submissions
      - in: query
        name: course_id
        description: The id of the contextual course for this API call
      - in: query
        name: user_id
        description: The ID of the user for which you want to see submissions
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Gradebook
      - History
      - Feed
  /courses/{course_id}/grading_periods:
    get:
      summary: List grading periods
      description: List grading periods.
      operationId: list-grading-periods
      x-api-path-slug: coursescourse-idgrading-periods-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Grading
      - Periods
    post:
      summary: Create a single grading period
      description: Create a single grading period.
      operationId: create-a-single-grading-period
      x-api-path-slug: coursescourse-idgrading-periods-post
      parameters:
      - in: query
        name: grading_periods[][end_date]
        description: no description
      - in: query
        name: grading_periods[][start_date]
        description: The date the grading period starts
      - in: query
        name: grading_periods[][weight]
        description: The percentage weight of how much the period should count toward
          the coursengrade
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Grading
      - Periods
  /courses/{course_id}/grading_periods/id:
    delete:
      summary: Delete a grading period
      description: Delete a grading period.
      operationId: delete-a-grading-period
      x-api-path-slug: coursescourse-idgrading-periodsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Grading
      - Periods
      - Id
    get:
      summary: Get a single grading period
      description: Get a single grading period.
      operationId: get-a-single-grading-period
      x-api-path-slug: coursescourse-idgrading-periodsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Grading
      - Periods
      - Id
    put:
      summary: Update a single grading period
      description: Update a single grading period.
      operationId: update-a-single-grading-period
      x-api-path-slug: coursescourse-idgrading-periodsid-put
      parameters:
      - in: query
        name: grading_periods[][end_date]
        description: no description
      - in: query
        name: grading_periods[][start_date]
        description: The date the grading period starts
      - in: query
        name: grading_periods[][weight]
        description: The percentage weight of how much the period should count toward
          the coursengrade
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Grading
      - Periods
      - Id
  /courses/{course_id}/grading_standards:
    get:
      summary: List the grading standards available in a context.
      description: List the grading standards available in a context..
      operationId: list-the-grading-standards-available-in-a-context
      x-api-path-slug: coursescourse-idgrading-standards-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Grading
      - Standards
    post:
      summary: Create a new grading standard
      description: Create a new grading standard.
      operationId: create-a-new-grading-standard
      x-api-path-slug: coursescourse-idgrading-standards-post
      parameters:
      - in: query
        name: grading_scheme_entry[][name]
        description: The name for an entry value within a GradingStandard that describes
          thenrange of the value e
      - in: query
        name: grading_scheme_entry[][value]
        description: The value for the name of the entry within a GradingStandard
      - in: query
        name: title
        description: The title for the Grading Standard
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Grading
      - Standards
  /courses/{course_id}/groups:
    get:
      summary: List the groups available in a context.
      description: List the groups available in a context..
      operationId: list-the-groups-available-in-a-context
      x-api-path-slug: coursescourse-idgroups-get
      parameters:
      - in: query
        name: only_own_groups
        description: Will only include groups that the user belongs to if this is
          set
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Groups
  /courses/{course_id}/group_categories:
    get:
      summary: List group categories for a context
      description: List group categories for a context.
      operationId: list-group-categories-for-a-context
      x-api-path-slug: coursescourse-idgroup-categories-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Group
      - Categories
    post:
      summary: Create a Group Category
      description: Create a group category.
      operationId: create-a-group-category
      x-api-path-slug: coursescourse-idgroup-categories-post
      parameters:
      - in: query
        name: auto_leader
        description: 'Assigns group leaders automatically when generating and allocating
          studentsnto groups Valid values are:nu201cfirstu201dnnthe first student
          to be allocated to a group is the leadernu201crandomu201dnna random student
          from all members is chosen as the leadernnn        n        n          Allowed
          values: first, random'
      - in: query
        name: create_group_count
        description: Create this number of groups (Course Only)
      - in: query
        name: group_limit
        description: Limit the maximum number of users in each group (Course Only)
      - in: query
        name: name
        description: Name of the group category
      - in: query
        name: self_signup
        description: Allow students to sign up for a group themselves (Course Only)
      - in: query
        name: split_group_count
        description: (Deprecated) Create this number of groups, and evenly distribute
          studentsnamong them
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Group
      - Categories
  /courses/{course_id}/live_assessments:
    get:
      summary: List live assessments
      description: List live assessments.
      operationId: list-live-assessments
      x-api-path-slug: coursescourse-idlive-assessments-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Live
      - Assessments
    post:
      summary: Create or find a live assessment
      description: Create or find a live assessment.
      operationId: create-or-find-a-live-assessment
      x-api-path-slug: coursescourse-idlive-assessments-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Live
      - Assessments
  /courses/{course_id}/live_assessments/assessment_id/results:
    get:
      summary: List live assessment results
      description: List live assessment results.
      operationId: list-live-assessment-results
      x-api-path-slug: coursescourse-idlive-assessmentsassessment-idresults-get
      parameters:
      - in: query
        name: user_id
        description: If set, restrict results to those for this user
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Live
      - Assessments
      - Assessment
      - Id
      - Results
    post:
      summary: Create live assessment results
      description: Create live assessment results.
      operationId: create-live-assessment-results
      x-api-path-slug: coursescourse-idlive-assessmentsassessment-idresults-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Live
      - Assessments
      - Assessment
      - Id
      - Results
  /courses/{course_id}/modules:
    get:
      summary: List modules
      description: List modules.
      operationId: list-modules
      x-api-path-slug: coursescourse-idmodules-get
      parameters:
      - in: query
        name: include[]
        description: 'u201citemsu201d: Return module items inline if possible'
      - in: query
        name: search_term
        description: The partial name of the modules (and module items, if include
          is specified) to match and return
      - in: query
        name: student_id
        description: Returns module completion information for the student with this
          id
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
    post:
      summary: Create a module
      description: Create a module.
      operationId: create-a-module
      x-api-path-slug: coursescourse-idmodules-post
      parameters:
      - in: query
        name: module[name]
        description: The name of the module
      - in: query
        name: module[position]
        description: The position of this module in the course (1-based)
      - in: query
        name: module[prerequisite_module_ids][]
        description: IDs of Modules that must be completed before this one is unlocked
      - in: query
        name: module[publish_final_grade]
        description: Whether to publish the student&#39;s final grade for the course
          uponncompletion of this module
      - in: query
        name: module[require_sequential_progress]
        description: Whether module items must be unlocked in order
      - in: query
        name: module[unlock_at]
        description: The date the module will unlock
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
  /courses/{course_id}/modules/id:
    delete:
      summary: Delete module
      description: Delete module.
      operationId: delete-module
      x-api-path-slug: coursescourse-idmodulesid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Id
    get:
      summary: Show module
      description: Show module.
      operationId: show-module
      x-api-path-slug: coursescourse-idmodulesid-get
      parameters:
      - in: query
        name: include[]
        description: 'u201citemsu201d: Return module items inline if possible'
      - in: query
        name: student_id
        description: Returns module completion information for the student with this
          id
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Id
    put:
      summary: Update a module
      description: Update a module.
      operationId: update-a-module
      x-api-path-slug: coursescourse-idmodulesid-put
      parameters:
      - in: query
        name: module[name]
        description: The name of the module
      - in: query
        name: module[position]
        description: The position of the module in the course (1-based)
      - in: query
        name: module[prerequisite_module_ids][]
        description: IDs of Modules that must be completed before this one is unlockednPrerequisite
          modules must precede this module (i
      - in: query
        name: module[published]
        description: Whether the module is published and visible to students
      - in: query
        name: module[publish_final_grade]
        description: Whether to publish the student&#39;s final grade for the course
          uponncompletion of this module
      - in: query
        name: module[require_sequential_progress]
        description: Whether module items must be unlocked in order
      - in: query
        name: module[unlock_at]
        description: The date the module will unlock
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Id
  /courses/{course_id}/modules/id/relock:
    put:
      summary: Re-lock module progressions
      description: Re-lock module progressions.
      operationId: relock-module-progressions
      x-api-path-slug: coursescourse-idmodulesidrelock-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Id
      - Relock
  /courses/{course_id}/modules/module_id/items:
    get:
      summary: List module items
      description: List module items.
      operationId: list-module-items
      x-api-path-slug: coursescourse-idmodulesmodule-iditems-get
      parameters:
      - in: query
        name: include[]
        description: If included, will return additional details specific to the contentnassociated
          with each item
      - in: query
        name: search_term
        description: The partial title of the items to match and return
      - in: query
        name: student_id
        description: Returns module completion information for the student with this
          id
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
    post:
      summary: Create a module item
      description: Create a module item.
      operationId: create-a-module-item
      x-api-path-slug: coursescourse-idmodulesmodule-iditems-post
      parameters:
      - in: query
        name: module_item[completion_requirement][min_score]
        description: Minimum score required to complete
      - in: query
        name: module_item[completion_requirement][type]
        description: Completion requirement for this module item
      - in: query
        name: module_item[content_id]
        description: The id of the content to link to the module item
      - in: query
        name: module_item[external_url]
        description: External url that the item points to
      - in: query
        name: module_item[indent]
        description: 0-based indent level; module items may be indented to show a
          hierarchy
      - in: query
        name: module_item[new_tab]
        description: Whether the external tool opens in a new tab
      - in: query
        name: module_item[page_url]
        description: Suffix for the linked wiki page (e
      - in: query
        name: module_item[position]
        description: The position of this item in the module (1-based)
      - in: query
        name: module_item[title]
        description: The name of the module item and associated content
      - in: query
        name: module_item[type]
        description: 'The type of content linked to the itemnn        n        n          Allowed
          values: File, Page, Discussion, Assignment, Quiz, SubHeader, ExternalUrl,
          ExternalTool'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
  /courses/{course_id}/modules/module_id/items/{id}:
    delete:
      summary: Delete module item
      description: Delete module item.
      operationId: delete-module-item
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
      - Id
    get:
      summary: Show module item
      description: Show module item.
      operationId: show-module-item
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsid-get
      parameters:
      - in: query
        name: include[]
        description: If included, will return additional details specific to the contentnassociated
          with this item
      - in: query
        name: student_id
        description: Returns module completion information for the student with this
          id
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
      - Id
    put:
      summary: Update a module item
      description: Update a module item.
      operationId: update-a-module-item
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsid-put
      parameters:
      - in: query
        name: module_item[completion_requirement][min_score]
        description: Minimum score required to complete, Required for completion_requirementntype
          &#39;min_score&#39;
      - in: query
        name: module_item[completion_requirement][type]
        description: Completion requirement for this module item
      - in: query
        name: module_item[external_url]
        description: External url that the item points to
      - in: query
        name: module_item[indent]
        description: 0-based indent level; module items may be indented to show a
          hierarchy
      - in: query
        name: module_item[module_id]
        description: Move this item to another module by specifying the target module
          id here
      - in: query
        name: module_item[new_tab]
        description: Whether the external tool opens in a new tab
      - in: query
        name: module_item[position]
        description: The position of this item in the module (1-based)
      - in: query
        name: module_item[published]
        description: Whether the module item is published and visible to students
      - in: query
        name: module_item[title]
        description: The name of the module item
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
      - Id
  /courses/{course_id}/modules/module_id/items/{id}/done:
    put:
      summary: Mark module item as done/not done
      description: Mark module item as done/not done.
      operationId: mark-module-item-as-donenot-done
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsiddone-put
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
      - Id
      - Done
  /courses/{course_id}/modules/module_id/items/{id}/mark_read:
    post:
      summary: Mark module item read
      description: Mark module item read.
      operationId: mark-module-item-read
      x-api-path-slug: coursescourse-idmodulesmodule-iditemsidmark-read-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Modules
      - Module
      - Id
      - Items
      - Id
      - Mark
      - Read
  /courses/{course_id}/module_item_sequence:
    get:
      summary: Get module item sequence
      description: Get module item sequence.
      operationId: get-module-item-sequence
      x-api-path-slug: coursescourse-idmodule-item-sequence-get
      parameters:
      - in: query
        name: asset_id
        description: The id of the asset (or the url in the case of a Page)
      - in: query
        name: asset_type
        description: The type of asset to find module sequence information for
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Module
      - Item
      - Sequence
  /courses/{course_id}/outcome_groups:
    get:
      summary: Get all outcome groups for context
      description: Get all outcome groups for context.
      operationId: get-all-outcome-groups-for-context
      x-api-path-slug: coursescourse-idoutcome-groups-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
  /courses/{course_id}/outcome_groups/id:
    delete:
      summary: Delete an outcome group
      description: Delete an outcome group.
      operationId: delete-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
    get:
      summary: Show an outcome group
      description: Show an outcome group.
      operationId: show-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
    put:
      summary: Update an outcome group
      description: Update an outcome group.
      operationId: update-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsid-put
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
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
  /courses/{course_id}/outcome_groups/id/import:
    post:
      summary: Import an outcome group
      description: Import an outcome group.
      operationId: import-an-outcome-group
      x-api-path-slug: coursescourse-idoutcome-groupsidimport-post
      parameters:
      - in: query
        name: source_outcome_group_id
        description: The ID of the source outcome group
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Import
  /courses/{course_id}/outcome_groups/id/outcomes:
    get:
      summary: List linked outcomes
      description: List linked outcomes.
      operationId: list-linked-outcomes
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomes-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Outcomes
    post:
      summary: Create/link an outcome
      description: Create/link an outcome.
      operationId: createlink-an-outcome
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomes-post
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
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Outcomes
  /courses/{course_id}/outcome_groups/id/outcomes/{outcome_id}:
    delete:
      summary: Unlink an outcome
      description: Unlink an outcome.
      operationId: unlink-an-outcome
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomesoutcome-id-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Outcomes
      - Outcome
      - Id
    put:
      summary: Create/link an outcome
      description: Create/link an outcome.
      operationId: createlink-an-outcome
      x-api-path-slug: coursescourse-idoutcome-groupsidoutcomesoutcome-id-put
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
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Outcomes
      - Outcome
      - Id
  /courses/{course_id}/outcome_groups/id/subgroups:
    get:
      summary: List subgroups
      description: List subgroups.
      operationId: list-subgroups
      x-api-path-slug: coursescourse-idoutcome-groupsidsubgroups-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Subgroups
    post:
      summary: Create a subgroup
      description: Create a subgroup.
      operationId: create-a-subgroup
      x-api-path-slug: coursescourse-idoutcome-groupsidsubgroups-post
      parameters:
      - in: query
        name: description
        description: The description of the new outcome group
      - in: query
        name: title
        description: The title of the new outcome group
      - in: query
        name: vendor_guid
        description: A custom GUID for the learning standard
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Groups
      - Id
      - Subgroups
  /courses/{course_id}/outcome_group_links:
    get:
      summary: Get all outcome links for context
      description: Get all outcome links for context.
      operationId: get-all-outcome-links-for-context
      x-api-path-slug: coursescourse-idoutcome-group-links-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Group
      - Links
  /courses/{course_id}/outcome_results:
    get:
      summary: Get outcome results
      description: Get outcome results.
      operationId: get-outcome-results
      x-api-path-slug: coursescourse-idoutcome-results-get
      parameters:
      - in: query
        name: include[]
        description: String, u201calignmentsu201d|u201coutcomesu201d|u201coutcomes
      - in: query
        name: outcome_ids[]
        description: If specified, only the outcomes whose ids are given will be included
          in thenresults
      - in: query
        name: user_ids[]
        description: If specified, only the users whose ids are given will be included
          in thenresults
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Results
  /courses/{course_id}/outcome_rollups:
    get:
      summary: Get outcome result rollups
      description: Get outcome result rollups.
      operationId: get-outcome-result-rollups
      x-api-path-slug: coursescourse-idoutcome-rollups-get
      parameters:
      - in: query
        name: aggregate
        description: If specified, instead of returning one rollup for each user,
          all the usernrollups will be combined into one rollup for the course that
          will containnthe average rollup score for each outcome
      - in: query
        name: include[]
        description: String, u201ccoursesu201d|u201coutcomesu201d|u201coutcomes
      - in: query
        name: outcome_ids[]
        description: If specified, only the outcomes whose ids are given will be included
          in thenresults
      - in: query
        name: user_ids[]
        description: If specified, only the users whose ids are given will be included
          in thenresults or used in an aggregate result
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Outcome
      - Rollups
  /courses/{course_id}/pages:
    get:
      summary: List pages
      description: List pages.
      operationId: list-pages
      x-api-path-slug: coursescourse-idpages-get
      parameters:
      - in: query
        name: order
        description: The sorting order
      - in: query
        name: published
        description: If true, include only published paqes
      - in: query
        name: search_term
        description: The partial title of the pages to match and return
      - in: query
        name: sort
        description: Sort results by this field
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
    post:
      summary: Create page
      description: Create page.
      operationId: create-page
      x-api-path-slug: coursescourse-idpages-post
      parameters:
      - in: query
        name: wiki_page[body]
        description: The content for the new page
      - in: query
        name: wiki_page[editing_roles]
        description: Which user roles are allowed to edit this page
      - in: query
        name: wiki_page[front_page]
        description: Set an unhidden page as the front page (if true)
      - in: query
        name: wiki_page[notify_of_update]
        description: Whether participants should be notified when this page changes
      - in: query
        name: wiki_page[published]
        description: Whether the page is published (true) or draft state (false)
      - in: query
        name: wiki_page[title]
        description: The title for the new page
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
  /courses/{course_id}/pages/url:
    delete:
      summary: Delete page
      description: Delete page.
      operationId: delete-page
      x-api-path-slug: coursescourse-idpagesurl-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
    get:
      summary: Show page
      description: Show page.
      operationId: show-page
      x-api-path-slug: coursescourse-idpagesurl-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
    put:
      summary: Update/create page
      description: Update/create page.
      operationId: updatecreate-page
      x-api-path-slug: coursescourse-idpagesurl-put
      parameters:
      - in: query
        name: wiki_page[body]
        description: The content for the new page
      - in: query
        name: wiki_page[editing_roles]
        description: Which user roles are allowed to edit this page
      - in: query
        name: wiki_page[front_page]
        description: Set an unhidden page as the front page (if true)
      - in: query
        name: wiki_page[notify_of_update]
        description: Whether participants should be notified when this page changes
      - in: query
        name: wiki_page[published]
        description: Whether the page is published (true) or draft state (false)
      - in: query
        name: wiki_page[title]
        description: The title for the new page
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
  /courses/{course_id}/pages/url/revisions:
    get:
      summary: List revisions
      description: List revisions.
      operationId: list-revisions
      x-api-path-slug: coursescourse-idpagesurlrevisions-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Pages
      - Url
      - Revisions
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