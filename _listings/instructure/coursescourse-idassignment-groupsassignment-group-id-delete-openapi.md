---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Destroy an Assignment Group
  description: Destroy an assignment group.
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