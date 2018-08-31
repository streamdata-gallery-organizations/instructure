---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API List your groups
  description: List your groups.
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
  /courses/{course_id}/pages/url/revisions/latest:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: coursescourse-idpagesurlrevisionslatest-get
      parameters:
      - in: query
        name: summary
        description: If set, exclude page content from results
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
      - Latest
  /courses/{course_id}/pages/url/revisions/{revision_id}:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: coursescourse-idpagesurlrevisionsrevision-id-get
      parameters:
      - in: query
        name: summary
        description: If set, exclude page content from results
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
      - Revision
      - Id
    post:
      summary: Revert to revision
      description: Revert to revision.
      operationId: revert-to-revision
      x-api-path-slug: coursescourse-idpagesurlrevisionsrevision-id-post
      parameters:
      - in: query
        name: revision_id
        description: The revision to revert to (use the List Revisions API to see
          available revisions)
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
      - Revision
      - Id
  /courses/{course_id}/preview_html:
    post:
      summary: Preview processed html
      description: Preview processed html.
      operationId: preview-processed-html
      x-api-path-slug: coursescourse-idpreview-html-post
      parameters:
      - in: query
        name: html
        description: The html content to process
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Preview
      - Html
  /courses/{course_id}/quizzes:
    get:
      summary: List quizzes in a course
      description: List quizzes in a course.
      operationId: list-quizzes-in-a-course
      x-api-path-slug: coursescourse-idquizzes-get
      parameters:
      - in: query
        name: search_term
        description: The partial title of the quizzes to match and return
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
    post:
      summary: Create a quiz
      description: Create a quiz.
      operationId: create-a-quiz
      x-api-path-slug: coursescourse-idquizzes-post
      parameters:
      - in: query
        name: quiz[access_code]
        description: Restricts access to the quiz with a password
      - in: query
        name: quiz[allowed_attempts]
        description: Number of times a student is allowed to take a quiz
      - in: query
        name: quiz[assignment_group_id]
        description: The assignment group id to put the assignment in
      - in: query
        name: quiz[cant_go_back]
        description: Only valid if one_question_at_a_time=true If true, questions
          are lockednafter answering
      - in: query
        name: quiz[description]
        description: A description of the quiz
      - in: query
        name: quiz[due_at]
        description: The day/time the quiz is due
      - in: query
        name: quiz[hide_correct_answers_at]
        description: Only valid if show_correct_answers=true If set, the correct answers
          willnstop being visible once this date has passed
      - in: query
        name: quiz[hide_results]
        description: Dictates whether or not quiz results are hidden from students
      - in: query
        name: quiz[ip_filter]
        description: Restricts access to the quiz to computers in a specified IP range
      - in: query
        name: quiz[lock_at]
        description: The day/time the quiz is locked for students
      - in: query
        name: quiz[one_question_at_a_time]
        description: If true, shows quiz to student one question at a time
      - in: query
        name: quiz[one_time_results]
        description: Whether students should be prevented from viewing their quiz
          results pastnthe first time (right after they turn the quiz in
      - in: query
        name: quiz[published]
        description: Whether the quiz should have a draft state of published or unpublished
      - in: query
        name: quiz[quiz_type]
        description: The type of quiz
      - in: query
        name: quiz[scoring_policy]
        description: Required and only valid if allowed_attempts &gt; 1
      - in: query
        name: quiz[show_correct_answers]
        description: Only valid if hide_results=null If false, hides correct answers
          fromnstudents when quiz results are viewed
      - in: query
        name: quiz[show_correct_answers_at]
        description: Only valid if show_correct_answers=true If set, the correct answers
          will benvisible by students only after this date, otherwise the correct
          answers arenvisible once the student hands in their quiz submission
      - in: query
        name: quiz[show_correct_answers_last_attempt]
        description: Only valid if show_correct_answers=true and allowed_attempts
          &gt; 1 Ifntrue, hides correct answers from students when quiz results are
          viewednuntil they submit the last attempt for the quiz
      - in: query
        name: quiz[shuffle_answers]
        description: If true, quiz answers for multiple choice questions will be randomized
          forneach student
      - in: query
        name: quiz[time_limit]
        description: Time limit to take this quiz, in minutes
      - in: query
        name: quiz[title]
        description: The quiz title
      - in: query
        name: quiz[unlock_at]
        description: The day/time the quiz is unlocked for students
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
  /courses/{course_id}/quizzes/assignment_overrides:
    get:
      summary: Retrieve assignment-overridden dates for quizzes
      description: Retrieve assignment-overridden dates for quizzes.
      operationId: retrieve-assignmentoverridden-dates-for-quizzes
      x-api-path-slug: coursescourse-idquizzesassignment-overrides-get
      parameters:
      - in: query
        name: quiz_assignment_overrides[0][quiz_ids][]
        description: An array of quiz IDs
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Assignment
      - Overrides
  /courses/{course_id}/quizzes/id:
    delete:
      summary: Delete a quiz
      description: Delete a quiz.
      operationId: delete-a-quiz
      x-api-path-slug: coursescourse-idquizzesid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Id
    get:
      summary: Get a single quiz
      description: Get a single quiz.
      operationId: get-a-single-quiz
      x-api-path-slug: coursescourse-idquizzesid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Id
    put:
      summary: Edit a quiz
      description: Edit a quiz.
      operationId: edit-a-quiz
      x-api-path-slug: coursescourse-idquizzesid-put
      parameters:
      - in: query
        name: quiz[notify_of_update]
        description: If true, notifies users that the quiz has changed
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Id
  /courses/{course_id}/quizzes/id/reorder:
    post:
      summary: Reorder quiz items
      description: Reorder quiz items.
      operationId: reorder-quiz-items
      x-api-path-slug: coursescourse-idquizzesidreorder-post
      parameters:
      - in: query
        name: order[][id]
        description: The associated item&#39;s unique identifier
      - in: query
        name: order[][type]
        description: 'The type of item is either &#39;question&#39; or &#39;group&#39;nn        n        n          Allowed
          values: question, group'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Id
      - Reorder
  /courses/{course_id}/quizzes/id/submission_users/message:
    post:
      summary: Send a message to unsubmitted or submitted users for the quiz
      description: Send a message to unsubmitted or submitted users for the quiz.
      operationId: send-a-message-to-unsubmitted-or-submitted-users-for-the-quiz
      x-api-path-slug: coursescourse-idquizzesidsubmission-usersmessage-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Id
      - Submission
      - Users
      - Message
  /courses/{course_id}/quizzes/id/validate_access_code:
    post:
      summary: Validate quiz access code
      description: Validate quiz access code.
      operationId: validate-quiz-access-code
      x-api-path-slug: coursescourse-idquizzesidvalidate-access-code-post
      parameters:
      - in: query
        name: access_code
        description: The access code being validated
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Id
      - Validate
      - Access
      - Code
  /courses/{course_id}/quizzes/quiz_id/extensions:
    post:
      summary: Set extensions for student quiz submissions
      description: Set extensions for student quiz submissions.
      operationId: set-extensions-for-student-quiz-submissions
      x-api-path-slug: coursescourse-idquizzesquiz-idextensions-post
      parameters:
      - in: query
        name: extend_from_end_at
        description: The number of minutes to extend the quiz beyond the quiz&#39;s
          currentnending time
      - in: query
        name: extend_from_now
        description: The number of minutes to extend the quiz from the current time
      - in: query
        name: extra_attempts
        description: Number of times the student is allowed to re-take the quiz over
          thenmultiple-attempt limit
      - in: query
        name: extra_time
        description: The number of extra minutes to allow for all attempts
      - in: query
        name: manually_unlocked
        description: Allow the student to take the quiz even if it&#39;s locked for
          everyonenelse
      - in: query
        name: user_id
        description: The ID of the user we want to add quiz extensions for
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Extensions
  /courses/{course_id}/quizzes/quiz_id/groups:
    post:
      summary: Create a question group
      description: Create a question group.
      operationId: create-a-question-group
      x-api-path-slug: coursescourse-idquizzesquiz-idgroups-post
      parameters:
      - in: query
        name: quiz_groups[][assessment_question_bank_id]
        description: The id of the assessment question bank to pull questions from
      - in: query
        name: quiz_groups[][name]
        description: The name of the question group
      - in: query
        name: quiz_groups[][pick_count]
        description: The number of questions to randomly select for this group
      - in: query
        name: quiz_groups[][question_points]
        description: The number of points to assign to each question in the group
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
  /courses/{course_id}/quizzes/quiz_id/groups/{id}:
    delete:
      summary: Delete a question group
      description: Delete a question group.
      operationId: delete-a-question-group
      x-api-path-slug: coursescourse-idquizzesquiz-idgroupsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
      - Id
    get:
      summary: Get a single quiz group
      description: Get a single quiz group.
      operationId: get-a-single-quiz-group
      x-api-path-slug: coursescourse-idquizzesquiz-idgroupsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
      - Id
    put:
      summary: Update a question group
      description: Update a question group.
      operationId: update-a-question-group
      x-api-path-slug: coursescourse-idquizzesquiz-idgroupsid-put
      parameters:
      - in: query
        name: quiz_groups[][name]
        description: The name of the question group
      - in: query
        name: quiz_groups[][pick_count]
        description: The number of questions to randomly select for this group
      - in: query
        name: quiz_groups[][question_points]
        description: The number of points to assign to each question in the group
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
      - Id
  /courses/{course_id}/quizzes/quiz_id/groups/{id}/reorder:
    post:
      summary: Reorder question groups
      description: Reorder question groups.
      operationId: reorder-question-groups
      x-api-path-slug: coursescourse-idquizzesquiz-idgroupsidreorder-post
      parameters:
      - in: query
        name: order[][id]
        description: The associated item&#39;s unique identifier
      - in: query
        name: order[][type]
        description: 'The type of item is always &#39;question&#39; for a groupnn        n        n          Allowed
          values: question'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Groups
      - Id
      - Reorder
  /courses/{course_id}/quizzes/quiz_id/ip_filters:
    get:
      summary: Get available quiz IP filters.
      description: Get available quiz ip filters..
      operationId: get-available-quiz-ip-filters
      x-api-path-slug: coursescourse-idquizzesquiz-idip-filters-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Ip
      - Filters
  /courses/{course_id}/quizzes/quiz_id/questions:
    get:
      summary: List questions in a quiz or a submission
      description: List questions in a quiz or a submission.
      operationId: list-questions-in-a-quiz-or-a-submission
      x-api-path-slug: coursescourse-idquizzesquiz-idquestions-get
      parameters:
      - in: query
        name: quiz_submission_attempt
        description: The attempt of the submission you want the questions for
      - in: query
        name: quiz_submission_id
        description: If specified, the endpoint will return the questions that were
          presentednfor that submission
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Questions
    post:
      summary: Create a single quiz question
      description: Create a single quiz question.
      operationId: create-a-single-quiz-question
      x-api-path-slug: coursescourse-idquizzesquiz-idquestions-post
      parameters:
      - in: query
        name: question[answers]
        description: no description
      - in: query
        name: question[correct_comments]
        description: The comment to display if the student answers the question correctly
      - in: query
        name: question[incorrect_comments]
        description: The comment to display if the student answers incorrectly
      - in: query
        name: question[neutral_comments]
        description: The comment to display regardless of how the student answered
      - in: query
        name: question[points_possible]
        description: The maximum amount of points received for answering this questionncorrectly
      - in: query
        name: question[position]
        description: The order in which the question will be displayed in the quiz
          in relationnto other questions
      - in: query
        name: question[question_name]
        description: The name of the question
      - in: query
        name: question[question_text]
        description: The text of the question
      - in: query
        name: question[question_type]
        description: The type of question
      - in: query
        name: question[quiz_group_id]
        description: The id of the quiz group to assign the question to
      - in: query
        name: question[text_after_answers]
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Questions
  /courses/{course_id}/quizzes/quiz_id/questions/{id}:
    delete:
      summary: Delete a quiz question
      description: Delete a quiz question.
      operationId: delete-a-quiz-question
      x-api-path-slug: coursescourse-idquizzesquiz-idquestionsid-delete
      parameters:
      - in: query
        name: id
        description: The quiz question&#39;s unique identifier
      - in: query
        name: quiz_id
        description: The associated quiz&#39;s unique identifier
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Questions
      - Id
    get:
      summary: Get a single quiz question
      description: Get a single quiz question.
      operationId: get-a-single-quiz-question
      x-api-path-slug: coursescourse-idquizzesquiz-idquestionsid-get
      parameters:
      - in: query
        name: id
        description: The quiz question unique identifier
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Questions
      - Id
    put:
      summary: Update an existing quiz question
      description: Update an existing quiz question.
      operationId: update-an-existing-quiz-question
      x-api-path-slug: coursescourse-idquizzesquiz-idquestionsid-put
      parameters:
      - in: query
        name: id
        description: The quiz question&#39;s unique identifier
      - in: query
        name: question[answers]
        description: no description
      - in: query
        name: question[correct_comments]
        description: The comment to display if the student answers the question correctly
      - in: query
        name: question[incorrect_comments]
        description: The comment to display if the student answers incorrectly
      - in: query
        name: question[neutral_comments]
        description: The comment to display regardless of how the student answered
      - in: query
        name: question[points_possible]
        description: The maximum amount of points received for answering this questionncorrectly
      - in: query
        name: question[position]
        description: The order in which the question will be displayed in the quiz
          in relationnto other questions
      - in: query
        name: question[question_name]
        description: The name of the question
      - in: query
        name: question[question_text]
        description: The text of the question
      - in: query
        name: question[question_type]
        description: The type of question
      - in: query
        name: question[quiz_group_id]
        description: The id of the quiz group to assign the question to
      - in: query
        name: question[text_after_answers]
        description: no description
      - in: query
        name: quiz_id
        description: The associated quiz&#39;s unique identifier
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Questions
      - Id
  /courses/{course_id}/quizzes/quiz_id/reports:
    get:
      summary: Retrieve all quiz reports
      description: Retrieve all quiz reports.
      operationId: retrieve-all-quiz-reports
      x-api-path-slug: coursescourse-idquizzesquiz-idreports-get
      parameters:
      - in: query
        name: includes_all_versions
        description: Whether to retrieve reports that consider all the submissions
          or only thenmost recent
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Reports
    post:
      summary: Create a quiz report
      description: Create a quiz report.
      operationId: create-a-quiz-report
      x-api-path-slug: coursescourse-idquizzesquiz-idreports-post
      parameters:
      - in: query
        name: include
        description: Whether the output should include documents for the file and/or
          progressnobjects associated with this report
      - in: query
        name: quiz_report[includes_all_versions]
        description: Whether the report should consider all submissions or only the
          most recent
      - in: query
        name: quiz_report[report_type]
        description: The type of report to be generated
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Reports
  /courses/{course_id}/quizzes/quiz_id/reports/{id}:
    delete:
      summary: Abort the generation of a report, or remove a previously generated
        one
      description: Abort the generation of a report, or remove a previously generated
        one.
      operationId: abort-the-generation-of-a-report-or-remove-a-previously-generated-one
      x-api-path-slug: coursescourse-idquizzesquiz-idreportsid-delete
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Reports
      - Id
    get:
      summary: Get a quiz report
      description: Get a quiz report.
      operationId: get-a-quiz-report
      x-api-path-slug: coursescourse-idquizzesquiz-idreportsid-get
      parameters:
      - in: query
        name: include
        description: Whether the output should include documents for the file and/or
          progressnobjects associated with this report
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Reports
      - Id
  /courses/{course_id}/quizzes/quiz_id/statistics:
    get:
      summary: Fetching the latest quiz statistics
      description: Fetching the latest quiz statistics.
      operationId: fetching-the-latest-quiz-statistics
      x-api-path-slug: coursescourse-idquizzesquiz-idstatistics-get
      parameters:
      - in: query
        name: all_versions
        description: Whether the statistics report should include all submissions
          attempts
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Statistics
  /courses/{course_id}/quizzes/quiz_id/submissions:
    get:
      summary: Get all quiz submissions.
      description: Get all quiz submissions..
      operationId: get-all-quiz-submissions
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissions-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the quiz submission
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
    post:
      summary: Create the quiz submission (start a quiz-taking session)
      description: Create the quiz submission (start a quiz-taking session).
      operationId: create-the-quiz-submission-start-a-quiztaking-session
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissions-post
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: preview
        description: Whether this should be a preview QuizSubmission and not count
          towards thenuser&#39;s course record
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
  /courses/{course_id}/quizzes/quiz_id/submissions/self/files:
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsselffiles-post
      parameters:
      - in: query
        name: name
        description: The name of the quiz submission file
      - in: query
        name: on_duplicate
        description: How to handle duplicate names
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Self
      - Files
  /courses/{course_id}/quizzes/quiz_id/submissions/{id}:
    get:
      summary: Get a single quiz submission.
      description: Get a single quiz submission..
      operationId: get-a-single-quiz-submission
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsid-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the quiz submission
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
    put:
      summary: Update student question scores and comments.
      description: Update student question scores and comments..
      operationId: update-student-question-scores-and-comments
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsid-put
      parameters:
      - in: query
        name: attempt
        description: The attempt number of the quiz submission that should be updated
      - in: query
        name: fudge_points
        description: Amount of positive or negative points to fudge the total score
          by
      - in: query
        name: questions
        description: A set of scores and comments for each question answered by the
          student
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
  /courses/{course_id}/quizzes/quiz_id/submissions/{id}/complete:
    post:
      summary: Complete the quiz submission (turn it in).
      description: Complete the quiz submission (turn it in)..
      operationId: complete-the-quiz-submission-turn-it-in
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsidcomplete-post
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: attempt
        description: The attempt number of the quiz submission that should be completed
      - in: query
        name: validation_token
        description: The unique validation token you received when this Quiz Submission
          wasncreated
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
      - Complete
  /courses/{course_id}/quizzes/quiz_id/submissions/{id}/events:
    get:
      summary: Retrieve captured events
      description: Retrieve captured events.
      operationId: retrieve-captured-events
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsidevents-get
      parameters:
      - in: query
        name: attempt
        description: The specific submission attempt to look up the events for
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
      - Events
    post:
      summary: Submit captured events
      description: Submit captured events.
      operationId: submit-captured-events
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsidevents-post
      parameters:
      - in: query
        name: quiz_submission_events[]
        description: The submission events to be recorded
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
      - Events
  /courses/{course_id}/quizzes/quiz_id/submissions/{id}/time:
    get:
      summary: Get current quiz submission times.
      description: Get current quiz submission times..
      operationId: get-current-quiz-submission-times
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsidtime-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
      - Time
  /courses/{course_id}/quiz_extensions:
    post:
      summary: Set extensions for student quiz submissions
      description: Set extensions for student quiz submissions.
      operationId: set-extensions-for-student-quiz-submissions
      x-api-path-slug: coursescourse-idquiz-extensions-post
      parameters:
      - in: query
        name: extend_from_end_at
        description: The number of minutes to extend the quiz beyond the quiz&#39;s
          currentnending time
      - in: query
        name: extend_from_now
        description: The number of minutes to extend the quiz from the current time
      - in: query
        name: extra_attempts
        description: Number of times the student is allowed to re-take the quiz over
          thenmultiple-attempt limit
      - in: query
        name: extra_time
        description: The number of extra minutes to allow for all attempts
      - in: query
        name: manually_unlocked
        description: Allow the student to take the quiz even if it&#39;s locked for
          everyonenelse
      - in: query
        name: user_id
        description: The ID of the user we want to add quiz extensions for
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quiz
      - Extensions
  /courses/{course_id}/recent_students:
    get:
      summary: List recently logged in students
      description: List recently logged in students.
      operationId: list-recently-logged-in-students
      x-api-path-slug: coursescourse-idrecent-students-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Recent
      - Students
  /courses/{course_id}/reset_content:
    post:
      summary: Reset a course
      description: Reset a course.
      operationId: reset-a-course
      x-api-path-slug: coursescourse-idreset-content-post
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Reset
      - Content
  /courses/{course_id}/root_outcome_group:
    get:
      summary: Redirect to root outcome group for context
      description: Redirect to root outcome group for context.
      operationId: redirect-to-root-outcome-group-for-context
      x-api-path-slug: coursescourse-idroot-outcome-group-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Root
      - Outcome
      - Group
  /courses/{course_id}/search_users:
    get:
      summary: List users in course
      description: List users in course.
      operationId: list-users-in-course
      x-api-path-slug: coursescourse-idsearch-users-get
      parameters:
      - in: query
        name: enrollment_role
        description: Deprecated When set, only return users enrolled with the specifiedncourse-level
          role
      - in: query
        name: enrollment_role_id
        description: When set, only return courses where the user is enrolled with
          the specifiedncourse-level role
      - in: query
        name: enrollment_state[]
        description: When set, only return users where the enrollment workflow state
          is of onenof the given types
      - in: query
        name: enrollment_type[]
        description: When set, only return users where the user is enrolled as this
          type
      - in: query
        name: include[]
        description: 'u201cemailu201d: Optional user email'
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      - in: query
        name: user_id
        description: If included, the user will be queried and if the user is part
          of the usersnset, the page parameter will be modified so that the page containingnuser_id
          will be returned
      - in: query
        name: user_ids[]
        description: If included, the course users set will only include users with
          IDsnspecified by the param
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Search
      - Users
  /courses/{course_id}/sections:
    get:
      summary: List course sections
      description: List course sections.
      operationId: list-course-sections
      x-api-path-slug: coursescourse-idsections-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cstudentsu201d: Associations to include with the group'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Sections
    post:
      summary: Create course section
      description: Create course section.
      operationId: create-course-section
      x-api-path-slug: coursescourse-idsections-post
      parameters:
      - in: query
        name: course_section[end_at]
        description: Section end date in ISO8601 format
      - in: query
        name: course_section[name]
        description: The name of the section
      - in: query
        name: course_section[restrict_enrollments_to_section_dates]
        description: Set to true to restrict user enrollments to the start and end
          dates of thensection
      - in: query
        name: course_section[sis_section_id]
        description: The sis ID of the section
      - in: query
        name: course_section[start_at]
        description: Section start date in ISO8601 format, e
      - in: query
        name: enable_sis_reactivation
        description: When true, will first try to re-activate a deleted section with
          matchingnsis_section_id if possible
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Sections
  /courses/{course_id}/sections/id:
    get:
      summary: Get section information
      description: Get section information.
      operationId: get-section-information
      x-api-path-slug: coursescourse-idsectionsid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Sections
      - Id
  /courses/{course_id}/settings:
    get:
      summary: Get course settings
      description: Get course settings.
      operationId: get-course-settings
      x-api-path-slug: coursescourse-idsettings-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Settings
    put:
      summary: Update course settings
      description: Update course settings.
      operationId: update-course-settings
      x-api-path-slug: coursescourse-idsettings-put
      parameters:
      - in: query
        name: allow_student_discussion_editing
        description: Let students edit or delete their own discussion posts
      - in: query
        name: allow_student_discussion_topics
        description: Let students create discussion topics
      - in: query
        name: allow_student_forum_attachments
        description: Let students attach files to discussions
      - in: query
        name: allow_student_organized_groups
        description: Let students organize their own groups
      - in: query
        name: hide_distribution_graphs
        description: Hide grade distribution graphs from students
      - in: query
        name: hide_final_grades
        description: Hide totals in student grades summary
      - in: query
        name: lock_all_announcements
        description: Disable comments on announcements
      - in: query
        name: restrict_student_future_view
        description: Restrict students from viewing courses before start date
      - in: query
        name: restrict_student_past_view
        description: Restrict students from viewing courses after end date
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Settings
  /courses/{course_id}/students:
    get:
      summary: List students
      description: List students.
      operationId: list-students
      x-api-path-slug: coursescourse-idstudents-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Students
  /courses/{course_id}/students/submissions:
    get:
      summary: List submissions for multiple assignments
      description: List submissions for multiple assignments.
      operationId: list-submissions-for-multiple-assignments
      x-api-path-slug: coursescourse-idstudentssubmissions-get
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
      - Courses
      - Course
      - Id
      - Students
      - Submissions
  /courses/{course_id}/submissions/update_grades:
    post:
      summary: Grade or comment on multiple submissions
      description: Grade or comment on multiple submissions.
      operationId: grade-or-comment-on-multiple-submissions
      x-api-path-slug: coursescourse-idsubmissionsupdate-grades-post
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
      - Submissions
      - Update
      - Grades
  /courses/{course_id}/tabs:
    get:
      summary: List available tabs for a course or group
      description: List available tabs for a course or group.
      operationId: list-available-tabs-for-a-course-or-group
      x-api-path-slug: coursescourse-idtabs-get
      parameters:
      - in: query
        name: include[]
        description: 'Optionally include external tool tabs in the returned list of
          tabs (Onlynhas effect for courses, not groups)nn        n        n          Allowed
          values: external'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Tabs
  /courses/{course_id}/tabs/tab_id:
    put:
      summary: Update a tab for a course
      description: Update a tab for a course.
      operationId: update-a-tab-for-a-course
      x-api-path-slug: coursescourse-idtabstab-id-put
      parameters:
      - in: query
        name: hidden
        description: no description
      - in: query
        name: position
        description: The new position of the tab, 1-based
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Tabs
      - Tab
      - Id
  /courses/{course_id}/todo:
    get:
      summary: Course TODO items
      description: Course todo items.
      operationId: course-todo-items
      x-api-path-slug: coursescourse-idtodo-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Todo
  /courses/{course_id}/usage_rights:
    delete:
      summary: Remove usage rights
      description: Remove usage rights.
      operationId: remove-usage-rights
      x-api-path-slug: coursescourse-idusage-rights-delete
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to remove associated usage rights from
      - in: query
        name: folder_ids[]
        description: List of ids of folders
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Usage
      - Rights
    put:
      summary: Set usage rights
      description: Set usage rights.
      operationId: set-usage-rights
      x-api-path-slug: coursescourse-idusage-rights-put
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to set usage rights for
      - in: query
        name: folder_ids[]
        description: List of ids of folders to search for files to set usage rights
          for
      - in: query
        name: publish
        description: Whether the file(s) or folder(s) should be published on save,
          provided thatnusage rights have been specified (set to `true` to publish
          on save)
      - in: query
        name: usage_rights[legal_copyright]
        description: The legal copyright line for the files
      - in: query
        name: usage_rights[license]
        description: The license that applies to the files
      - in: query
        name: usage_rights[use_justification]
        description: 'The intellectual property justification for using the files
          in Canvasnn        n        n          Allowed values: own_copyright, used_by_permission,
          fair_use, public_domain, creative_commons'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Usage
      - Rights
  /courses/{course_id}/users:
    get:
      summary: List users in course
      description: List users in course.
      operationId: list-users-in-course
      x-api-path-slug: coursescourse-idusers-get
      parameters:
      - in: query
        name: enrollment_role
        description: Deprecated When set, only return users enrolled with the specifiedncourse-level
          role
      - in: query
        name: enrollment_role_id
        description: When set, only return courses where the user is enrolled with
          the specifiedncourse-level role
      - in: query
        name: enrollment_state[]
        description: When set, only return users where the enrollment workflow state
          is of onenof the given types
      - in: query
        name: enrollment_type[]
        description: When set, only return users where the user is enrolled as this
          type
      - in: query
        name: include[]
        description: 'u201cemailu201d: Optional user email'
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      - in: query
        name: user_id
        description: If included, the user will be queried and if the user is part
          of the usersnset, the page parameter will be modified so that the page containingnuser_id
          will be returned
      - in: query
        name: user_ids[]
        description: If included, the course users set will only include users with
          IDsnspecified by the param
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Users
  /courses/{course_id}/users/id:
    get:
      summary: Get single user
      description: Get single user.
      operationId: get-single-user
      x-api-path-slug: coursescourse-idusersid-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Users
      - Id
  /courses/{id}:
    delete:
      summary: Conclude a course
      description: Conclude a course.
      operationId: conclude-a-course
      x-api-path-slug: coursesid-delete
      parameters:
      - in: query
        name: event
        description: The action to take on the course
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Id
    get:
      summary: Get a single course
      description: Get a single course.
      operationId: get-a-single-course
      x-api-path-slug: coursesid-get
      parameters:
      - in: query
        name: include[]
        description: 'u201call_coursesu201d: Also search recently deleted courses'
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Id
    put:
      summary: Update a course
      description: Update a course.
      operationId: update-a-course
      x-api-path-slug: coursesid-put
      parameters:
      - in: query
        name: course[account_id]
        description: The unique ID of the account to create to course under
      - in: query
        name: course[allow_student_forum_attachments]
        description: If true, students can attach files to forum posts
      - in: query
        name: course[allow_student_wiki_edits]
        description: If true, students will be able to modify the course wiki
      - in: query
        name: course[allow_wiki_comments]
        description: If true, course members will be able to comment on wiki pages
      - in: query
        name: course[apply_assignment_group_weights]
        description: Set to true to weight final grade based on assignment groups
          percentages
      - in: query
        name: course[course_code]
        description: The course code for the course
      - in: query
        name: course[course_format]
        description: Optional
      - in: query
        name: course[end_at]
        description: Course end date in ISO8601 format
      - in: query
        name: course[grading_standard_id]
        description: The grading standard id to set for the course
      - in: query
        name: course[hide_final_grades]
        description: If this option is set to true, the totals in student grades summary
          will benhidden
      - in: query
        name: course[integration_id]
        description: The unique Integration identifier
      - in: query
        name: course[is_public]
        description: Set to true if course if public
      - in: query
        name: course[license]
        description: The name of the licensing
      - in: query
        name: course[name]
        description: The name of the course
      - in: query
        name: course[open_enrollment]
        description: Set to true if the course is open enrollment
      - in: query
        name: course[public_description]
        description: A publicly visible description of the course
      - in: query
        name: course[public_syllabus]
        description: Set to true to make the course syllabus public
      - in: query
        name: course[restrict_enrollments_to_course_dates]
        description: Set to true to restrict user enrollments to the start and end
          dates of thencourse
      - in: query
        name: course[self_enrollment]
        description: Set to true if the course is self enrollment
      - in: query
        name: course[sis_course_id]
        description: The unique SIS identifier
      - in: query
        name: course[start_at]
        description: Course start date in ISO8601 format, e
      - in: query
        name: course[syllabus_body]
        description: The syllabus body for the course
      - in: query
        name: course[term_id]
        description: The unique ID of the term to create to course in
      - in: query
        name: offer
        description: If this option is set to true, the course will be available to
          studentsnimmediately
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Id
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
    put:
      summary: Create/link an outcome
      description: Create/link an outcome.
      operationId: createlink-an-outcome
      x-api-path-slug: globaloutcome-groupsidoutcomesoutcome-id-put
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
      - Outcome
      - Id
  /global/outcome_groups/{id}/subgroups:
    get:
      summary: List subgroups
      description: List subgroups.
      operationId: list-subgroups
      x-api-path-slug: globaloutcome-groupsidsubgroups-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Outcome
      - Groups
      - Id
      - Subgroups
    post:
      summary: Create a subgroup
      description: Create a subgroup.
      operationId: create-a-subgroup
      x-api-path-slug: globaloutcome-groupsidsubgroups-post
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
      - Global
      - Outcome
      - Groups
      - Id
      - Subgroups
  /global/root_outcome_group:
    get:
      summary: Redirect to root outcome group for context
      description: Redirect to root outcome group for context.
      operationId: redirect-to-root-outcome-group-for-context
      x-api-path-slug: globalroot-outcome-group-get
      responses:
        200:
          description: OK
      tags:
      - Global
      - Root
      - Outcome
      - Group
  /groups:
    post:
      summary: Create a group
      description: Create a group.
      operationId: create-a-group
      x-api-path-slug: groups-post
      parameters:
      - in: query
        name: description
        description: A description of the group
      - in: query
        name: is_public
        description: whether the group is public (applies only to community groups)
      - in: query
        name: join_level
        description: 'no descriptionnn        n        n          Allowed values:
          parent_context_auto_join, parent_context_request, invitation_only'
      - in: query
        name: name
        description: The name of the group
      - in: query
        name: storage_quota_mb
        description: The allowed file storage for the group, in megabytes
      responses:
        200:
          description: OK
      tags:
      - Groups
  /groups/{group_id}:
    delete:
      summary: Delete a group
      description: Delete a group.
      operationId: delete-a-group
      x-api-path-slug: groupsgroup-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
    get:
      summary: Get a single group
      description: Get a single group.
      operationId: get-a-single-group
      x-api-path-slug: groupsgroup-id-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cpermissionsu201d: Include permissions the current user
          has for the group'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
    put:
      summary: Edit a group
      description: Edit a group.
      operationId: edit-a-group
      x-api-path-slug: groupsgroup-id-put
      parameters:
      - in: query
        name: avatar_id
        description: The id of the attachment previously uploaded to the group that
          you wouldnlike to use as the avatar image for this group
      - in: query
        name: description
        description: A description of the group
      - in: query
        name: is_public
        description: Whether the group is public (applies only to community groups)
      - in: query
        name: join_level
        description: 'no descriptionnn        n        n          Allowed values:
          parent_context_auto_join, parent_context_request, invitation_only'
      - in: query
        name: members[]
        description: An array of user ids for users you would like in the group
      - in: query
        name: name
        description: The name of the group
      - in: query
        name: storage_quota_mb
        description: The allowed file storage for the group, in megabytes
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
  /groups/{group_id}/activity_stream:
    get:
      summary: Group activity stream
      description: Group activity stream.
      operationId: group-activity-stream
      x-api-path-slug: groupsgroup-idactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Activity
      - Stream
  /groups/{group_id}/activity_stream/summary:
    get:
      summary: Group activity stream summary
      description: Group activity stream summary.
      operationId: group-activity-stream-summary
      x-api-path-slug: groupsgroup-idactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Activity
      - Stream
      - Summary
  /groups/{group_id}/assignments/assignment_id/override:
    get:
      summary: Redirect to the assignment override for a group
      description: Redirect to the assignment override for a group.
      operationId: redirect-to-the-assignment-override-for-a-group
      x-api-path-slug: groupsgroup-idassignmentsassignment-idoverride-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Assignments
      - Assignment
      - Id
      - Override
  /groups/{group_id}/conferences:
    get:
      summary: List conferences
      description: List conferences.
      operationId: list-conferences
      x-api-path-slug: groupsgroup-idconferences-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Conferences
  /groups/{group_id}/content_exports:
    get:
      summary: List content exports
      description: List content exports.
      operationId: list-content-exports
      x-api-path-slug: groupsgroup-idcontent-exports-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Exports
    post:
      summary: Export content
      description: Export content.
      operationId: export-content
      x-api-path-slug: groupsgroup-idcontent-exports-post
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
      - Groups
      - Group
      - Id
      - Content
      - Exports
  /groups/{group_id}/content_exports/id:
    get:
      summary: Show content export
      description: Show content export.
      operationId: show-content-export
      x-api-path-slug: groupsgroup-idcontent-exportsid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Exports
      - Id
  /groups/{group_id}/content_licenses:
    get:
      summary: List licenses
      description: List licenses.
      operationId: list-licenses
      x-api-path-slug: groupsgroup-idcontent-licenses-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Licenses
  /groups/{group_id}/content_migrations:
    get:
      summary: List content migrations
      description: List content migrations.
      operationId: list-content-migrations
      x-api-path-slug: groupsgroup-idcontent-migrations-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
    post:
      summary: Create a content migration
      description: Create a content migration.
      operationId: create-a-content-migration
      x-api-path-slug: groupsgroup-idcontent-migrations-post
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
      - Groups
      - Group
      - Id
      - Content
      - Migrations
  /groups/{group_id}/content_migrations/content_migration_id/migration_issues:
    get:
      summary: List migration issues
      description: List migration issues.
      operationId: list-migration-issues
      x-api-path-slug: groupsgroup-idcontent-migrationscontent-migration-idmigration-issues-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
  /groups/{group_id}/content_migrations/content_migration_id/migration_issues/{id}:
    get:
      summary: Get a migration issue
      description: Get a migration issue.
      operationId: get-a-migration-issue
      x-api-path-slug: groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
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
      x-api-path-slug: groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-put
      parameters:
      - in: query
        name: workflow_state
        description: Set the workflow_state of the issue
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
      - Id
  /groups/{group_id}/content_migrations/id:
    get:
      summary: Get a content migration
      description: Get a content migration.
      operationId: get-a-content-migration
      x-api-path-slug: groupsgroup-idcontent-migrationsid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Id
    put:
      summary: Update a content migration
      description: Update a content migration.
      operationId: update-a-content-migration
      x-api-path-slug: groupsgroup-idcontent-migrationsid-put
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Id
  /groups/{group_id}/content_migrations/migrators:
    get:
      summary: List Migration Systems
      description: List migration systems.
      operationId: list-migration-systems
      x-api-path-slug: groupsgroup-idcontent-migrationsmigrators-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Content
      - Migrations
      - Migrators
  /groups/{group_id}/discussion_topics:
    get:
      summary: List discussion topics
      description: List discussion topics.
      operationId: list-discussion-topics
      x-api-path-slug: groupsgroup-iddiscussion-topics-get
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
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
    post:
      summary: Create a new discussion topic
      description: Create a new discussion topic.
      operationId: create-a-new-discussion-topic
      x-api-path-slug: groupsgroup-iddiscussion-topics-post
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
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
  /groups/{group_id}/discussion_topics/reorder:
    post:
      summary: Reorder pinned topics
      description: Reorder pinned topics.
      operationId: reorder-pinned-topics
      x-api-path-slug: groupsgroup-iddiscussion-topicsreorder-post
      parameters:
      - in: query
        name: order[]
        description: The ids of the pinned discussion topics in the desired order
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Reorder
  /groups/{group_id}/discussion_topics/topic_id:
    delete:
      summary: Delete a topic
      description: Delete a topic.
      operationId: delete-a-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
    get:
      summary: Get a single topic
      description: Get a single topic.
      operationId: get-a-single-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-id-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
    put:
      summary: Update a topic
      description: Update a topic.
      operationId: update-a-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-id-put
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
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
  /groups/{group_id}/discussion_topics/topic_id/entries:
    get:
      summary: List topic entries
      description: List topic entries.
      operationId: list-topic-entries
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identries-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
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
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identries-post
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
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
  /groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/rating:
    post:
      summary: Rate entry
      description: Rate entry.
      operationId: rate-entry
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idrating-post
      parameters:
      - in: query
        name: rating
        description: A rating to set on this entry
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Rating
  /groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/read:
    delete:
      summary: Mark entry as unread
      description: Mark entry as unread.
      operationId: mark-entry-as-unread
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idread-delete
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set the entry&#39;s forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
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
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idread-put
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set the entry&#39;s forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Read
  /groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/replies:
    get:
      summary: List entry replies
      description: List entry replies.
      operationId: list-entry-replies
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
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
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-post
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
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Replies
  /groups/{group_id}/discussion_topics/topic_id/entries/{id}:
    delete:
      summary: Delete an entry
      description: Delete an entry.
      operationId: delete-an-entry
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesid-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
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
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesid-put
      parameters:
      - in: query
        name: message
        description: The updated body of the entry
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Id
  /groups/{group_id}/discussion_topics/topic_id/entry_list:
    get:
      summary: List entries
      description: List entries.
      operationId: list-entries
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identry-list-get
      parameters:
      - in: query
        name: ids[]
        description: A list of entry ids to retrieve
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entry
      - List
  /groups/{group_id}/discussion_topics/topic_id/read:
    delete:
      summary: Mark topic as unread
      description: Mark topic as unread.
      operationId: mark-topic-as-unread
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idread-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
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
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idread-put
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
  /groups/{group_id}/discussion_topics/topic_id/read_all:
    delete:
      summary: Mark all entries as unread
      description: Mark all entries as unread.
      operationId: mark-all-entries-as-unread
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idread-all-delete
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set all of the entries&#39; forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
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
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idread-all-put
      parameters:
      - in: query
        name: forced_read_state
        description: A boolean value to set all of the entries&#39; forced_read_state
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Read
  /groups/{group_id}/discussion_topics/topic_id/subscribed:
    delete:
      summary: Unsubscribe from a topic
      description: Unsubscribe from a topic.
      operationId: unsubscribe-from-a-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idsubscribed-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
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
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idsubscribed-put
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Subscribed
  /groups/{group_id}/discussion_topics/topic_id/view:
    get:
      summary: Get the full topic
      description: Get the full topic.
      operationId: get-the-full-topic
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-idview-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - View
  /groups/{group_id}/external_feeds:
    get:
      summary: List external feeds
      description: List external feeds.
      operationId: list-external-feeds
      x-api-path-slug: groupsgroup-idexternal-feeds-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - External
      - Feeds
    post:
      summary: Create an external feed
      description: Create an external feed.
      operationId: create-an-external-feed
      x-api-path-slug: groupsgroup-idexternal-feeds-post
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
      - Groups
      - Group
      - Id
      - External
      - Feeds
  /groups/{group_id}/external_feeds/external_feed_id:
    delete:
      summary: Delete an external feed
      description: Delete an external feed.
      operationId: delete-an-external-feed
      x-api-path-slug: groupsgroup-idexternal-feedsexternal-feed-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - External
      - Feeds
      - External
      - Feed
      - Id
  /groups/{group_id}/files:
    get:
      summary: List files
      description: List files.
      operationId: list-files
      x-api-path-slug: groupsgroup-idfiles-get
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
      - Groups
      - Group
      - Id
      - Files
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: groupsgroup-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
  /groups/{group_id}/files/id:
    get:
      summary: Get file
      description: Get file.
      operationId: get-file
      x-api-path-slug: groupsgroup-idfilesid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
      - Id
  /groups/{group_id}/files/quota:
    get:
      summary: Get quota information
      description: Get quota information.
      operationId: get-quota-information
      x-api-path-slug: groupsgroup-idfilesquota-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Files
      - Quota
  /groups/{group_id}/folders:
    get:
      summary: List all folders
      description: List all folders.
      operationId: list-all-folders
      x-api-path-slug: groupsgroup-idfolders-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Folders
    post:
      summary: Create folder
      description: Create folder.
      operationId: create-folder
      x-api-path-slug: groupsgroup-idfolders-post
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
      - Groups
      - Group
      - Id
      - Folders
  /groups/{group_id}/folders/by_path:
    get:
      summary: Resolve path
      description: Resolve path.
      operationId: resolve-path
      x-api-path-slug: groupsgroup-idfoldersby-path-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Folders
      - By
      - Path
  /groups/{group_id}/folders/by_path/*full_path:
    get:
      summary: Resolve path
      description: Resolve path.
      operationId: resolve-path
      x-api-path-slug: groupsgroup-idfoldersby-pathfull-path-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Folders
      - By
      - Path
      - '*full'
      - Path
  /groups/{group_id}/folders/id:
    get:
      summary: Get folder
      description: Get folder.
      operationId: get-folder
      x-api-path-slug: groupsgroup-idfoldersid-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Folders
      - Id
  /groups/{group_id}/front_page:
    get:
      summary: Show front page
      description: Show front page.
      operationId: show-front-page
      x-api-path-slug: groupsgroup-idfront-page-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Front
      - Page
    put:
      summary: Update/create front page
      description: Update/create front page.
      operationId: updatecreate-front-page
      x-api-path-slug: groupsgroup-idfront-page-put
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
      - Groups
      - Group
      - Id
      - Front
      - Page
  /groups/{group_id}/invite:
    post:
      summary: Invite others to a group
      description: Invite others to a group.
      operationId: invite-others-to-a-group
      x-api-path-slug: groupsgroup-idinvite-post
      parameters:
      - in: query
        name: invitees[]
        description: An array of email addresses to be sent invitations
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Invite
  /groups/{group_id}/memberships:
    get:
      summary: List group memberships
      description: List group memberships.
      operationId: list-group-memberships
      x-api-path-slug: groupsgroup-idmemberships-get
      parameters:
      - in: query
        name: filter_states[]
        description: Only list memberships with the given workflow_states
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
    post:
      summary: Create a membership
      description: Create a membership.
      operationId: create-a-membership
      x-api-path-slug: groupsgroup-idmemberships-post
      parameters:
      - in: query
        name: user_id
        description: no description
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
  /groups/{group_id}/memberships/membership_id:
    delete:
      summary: Leave a group
      description: Leave a group.
      operationId: leave-a-group
      x-api-path-slug: groupsgroup-idmembershipsmembership-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
      - Membership
      - Id
    get:
      summary: Get a single group membership
      description: Get a single group membership.
      operationId: get-a-single-group-membership
      x-api-path-slug: groupsgroup-idmembershipsmembership-id-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
      - Membership
      - Id
    put:
      summary: Update a membership
      description: Update a membership.
      operationId: update-a-membership
      x-api-path-slug: groupsgroup-idmembershipsmembership-id-put
      parameters:
      - in: query
        name: moderator
        description: no description
      - in: query
        name: workflow_state
        description: 'Currently, the only allowed value is u201cacceptedu201dnn        n        n          Allowed
          values: accepted'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Memberships
      - Membership
      - Id
  /groups/{group_id}/pages:
    get:
      summary: List pages
      description: List pages.
      operationId: list-pages
      x-api-path-slug: groupsgroup-idpages-get
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
      - Groups
      - Group
      - Id
      - Pages
    post:
      summary: Create page
      description: Create page.
      operationId: create-page
      x-api-path-slug: groupsgroup-idpages-post
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
      - Groups
      - Group
      - Id
      - Pages
  /groups/{group_id}/pages/url:
    delete:
      summary: Delete page
      description: Delete page.
      operationId: delete-page
      x-api-path-slug: groupsgroup-idpagesurl-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
    get:
      summary: Show page
      description: Show page.
      operationId: show-page
      x-api-path-slug: groupsgroup-idpagesurl-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
    put:
      summary: Update/create page
      description: Update/create page.
      operationId: updatecreate-page
      x-api-path-slug: groupsgroup-idpagesurl-put
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
      - Groups
      - Group
      - Id
      - Pages
      - Url
  /groups/{group_id}/pages/url/revisions:
    get:
      summary: List revisions
      description: List revisions.
      operationId: list-revisions
      x-api-path-slug: groupsgroup-idpagesurlrevisions-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
  /groups/{group_id}/pages/url/revisions/latest:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: groupsgroup-idpagesurlrevisionslatest-get
      parameters:
      - in: query
        name: summary
        description: If set, exclude page content from results
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
      - Latest
  /groups/{group_id}/pages/url/revisions/{revision_id}:
    get:
      summary: Show revision
      description: Show revision.
      operationId: show-revision
      x-api-path-slug: groupsgroup-idpagesurlrevisionsrevision-id-get
      parameters:
      - in: query
        name: summary
        description: If set, exclude page content from results
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
      - Revision
      - Id
    post:
      summary: Revert to revision
      description: Revert to revision.
      operationId: revert-to-revision
      x-api-path-slug: groupsgroup-idpagesurlrevisionsrevision-id-post
      parameters:
      - in: query
        name: revision_id
        description: The revision to revert to (use the List Revisions API to see
          available revisions)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Pages
      - Url
      - Revisions
      - Revision
      - Id
  /groups/{group_id}/preview_html:
    post:
      summary: Preview processed html
      description: Preview processed html.
      operationId: preview-processed-html
      x-api-path-slug: groupsgroup-idpreview-html-post
      parameters:
      - in: query
        name: html
        description: The html content to process
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Preview
      - Html
  /groups/{group_id}/tabs:
    get:
      summary: List available tabs for a course or group
      description: List available tabs for a course or group.
      operationId: list-available-tabs-for-a-course-or-group
      x-api-path-slug: groupsgroup-idtabs-get
      parameters:
      - in: query
        name: include[]
        description: 'Optionally include external tool tabs in the returned list of
          tabs (Onlynhas effect for courses, not groups)nn        n        n          Allowed
          values: external'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Tabs
  /groups/{group_id}/usage_rights:
    delete:
      summary: Remove usage rights
      description: Remove usage rights.
      operationId: remove-usage-rights
      x-api-path-slug: groupsgroup-idusage-rights-delete
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to remove associated usage rights from
      - in: query
        name: folder_ids[]
        description: List of ids of folders
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Usage
      - Rights
    put:
      summary: Set usage rights
      description: Set usage rights.
      operationId: set-usage-rights
      x-api-path-slug: groupsgroup-idusage-rights-put
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to set usage rights for
      - in: query
        name: folder_ids[]
        description: List of ids of folders to search for files to set usage rights
          for
      - in: query
        name: publish
        description: Whether the file(s) or folder(s) should be published on save,
          provided thatnusage rights have been specified (set to `true` to publish
          on save)
      - in: query
        name: usage_rights[legal_copyright]
        description: The legal copyright line for the files
      - in: query
        name: usage_rights[license]
        description: The license that applies to the files
      - in: query
        name: usage_rights[use_justification]
        description: 'The intellectual property justification for using the files
          in Canvasnn        n        n          Allowed values: own_copyright, used_by_permission,
          fair_use, public_domain, creative_commons'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Usage
      - Rights
  /groups/{group_id}/users:
    get:
      summary: List groups users
      description: List groups users.
      operationId: list-groups-users
      x-api-path-slug: groupsgroup-idusers-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cavatar_urlu201d: Include users&#39; avatar_urls'
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
  /groups/{group_id}/users/user_id:
    delete:
      summary: Leave a group
      description: Leave a group.
      operationId: leave-a-group
      x-api-path-slug: groupsgroup-idusersuser-id-delete
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
      - User
      - Id
    get:
      summary: Get a single group membership
      description: Get a single group membership.
      operationId: get-a-single-group-membership
      x-api-path-slug: groupsgroup-idusersuser-id-get
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
      - User
      - Id
    put:
      summary: Update a membership
      description: Update a membership.
      operationId: update-a-membership
      x-api-path-slug: groupsgroup-idusersuser-id-put
      parameters:
      - in: query
        name: moderator
        description: no description
      - in: query
        name: workflow_state
        description: 'Currently, the only allowed value is u201cacceptedu201dnn        n        n          Allowed
          values: accepted'
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Users
      - User
      - Id
  /group_categories/{group_category_id}:
    delete:
      summary: Delete a Group Category
      description: Delete a group category.
      operationId: delete-a-group-category
      x-api-path-slug: group-categoriesgroup-category-id-delete
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
    get:
      summary: Get a single group category
      description: Get a single group category.
      operationId: get-a-single-group-category
      x-api-path-slug: group-categoriesgroup-category-id-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
    put:
      summary: Update a Group Category
      description: Update a group category.
      operationId: update-a-group-category
      x-api-path-slug: group-categoriesgroup-category-id-put
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
      - Group
      - Categories
      - Group
      - Category
      - Id
  /group_categories/{group_category_id}/assign_unassigned_members:
    post:
      summary: Assign unassigned members
      description: Assign unassigned members.
      operationId: assign-unassigned-members
      x-api-path-slug: group-categoriesgroup-category-idassign-unassigned-members-post
      parameters:
      - in: query
        name: sync
        description: The assigning is done asynchronously by default
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
      - Assign
      - Unassigned
      - Members
  /group_categories/{group_category_id}/groups:
    get:
      summary: List groups in group category
      description: List groups in group category.
      operationId: list-groups-in-group-category
      x-api-path-slug: group-categoriesgroup-category-idgroups-get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
      - Groups
    post:
      summary: Create a group
      description: Create a group.
      operationId: create-a-group
      x-api-path-slug: group-categoriesgroup-category-idgroups-post
      parameters:
      - in: query
        name: description
        description: A description of the group
      - in: query
        name: is_public
        description: whether the group is public (applies only to community groups)
      - in: query
        name: join_level
        description: 'no descriptionnn        n        n          Allowed values:
          parent_context_auto_join, parent_context_request, invitation_only'
      - in: query
        name: name
        description: The name of the group
      - in: query
        name: storage_quota_mb
        description: The allowed file storage for the group, in megabytes
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
      - Groups
  /group_categories/{group_category_id}/users:
    get:
      summary: List users in group category
      description: List users in group category.
      operationId: list-users-in-group-category
      x-api-path-slug: group-categoriesgroup-category-idusers-get
      parameters:
      - in: query
        name: search_term
        description: The partial name or full ID of the users to match and return
          in the resultsnlist
      - in: query
        name: unassigned
        description: Set this value to true if you wish only to search unassigned
          users in thengroup category
      responses:
        200:
          description: OK
      tags:
      - Group
      - Categories
      - Group
      - Category
      - Id
      - Users
  /polls:
    get:
      summary: List polls
      description: List polls.
      operationId: list-polls
      x-api-path-slug: polls-get
      responses:
        200:
          description: OK
      tags:
      - Polls
    post:
      summary: Create a single poll
      description: Create a single poll.
      operationId: create-a-single-poll
      x-api-path-slug: polls-post
      parameters:
      - in: query
        name: polls[][description]
        description: A brief description or instructions for the poll
      - in: query
        name: polls[][question]
        description: The title of the poll
      responses:
        200:
          description: OK
      tags:
      - Polls
  /polls/{id}:
    delete:
      summary: Delete a poll
      description: Delete a poll.
      operationId: delete-a-poll
      x-api-path-slug: pollsid-delete
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Id
    get:
      summary: Get a single poll
      description: Get a single poll.
      operationId: get-a-single-poll
      x-api-path-slug: pollsid-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Id
    put:
      summary: Update a single poll
      description: Update a single poll.
      operationId: update-a-single-poll
      x-api-path-slug: pollsid-put
      parameters:
      - in: query
        name: polls[][description]
        description: A brief description or instructions for the poll
      - in: query
        name: polls[][question]
        description: The title of the poll
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Id
  /polls/{poll_id}/poll_choices:
    get:
      summary: List poll choices in a poll
      description: List poll choices in a poll.
      operationId: list-poll-choices-in-a-poll
      x-api-path-slug: pollspoll-idpoll-choices-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Choices
    post:
      summary: Create a single poll choice
      description: Create a single poll choice.
      operationId: create-a-single-poll-choice
      x-api-path-slug: pollspoll-idpoll-choices-post
      parameters:
      - in: query
        name: poll_choices[][is_correct]
        description: Whether this poll choice is considered correct or not
      - in: query
        name: poll_choices[][position]
        description: The order this poll choice should be returned in the context
          it&#39;snsibling poll choices
      - in: query
        name: poll_choices[][text]
        description: The descriptive text of the poll choice
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Choices
  /polls/{poll_id}/poll_choices/id:
    delete:
      summary: Delete a poll choice
      description: Delete a poll choice.
      operationId: delete-a-poll-choice
      x-api-path-slug: pollspoll-idpoll-choicesid-delete
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Choices
      - Id
    get:
      summary: Get a single poll choice
      description: Get a single poll choice.
      operationId: get-a-single-poll-choice
      x-api-path-slug: pollspoll-idpoll-choicesid-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Choices
      - Id
    put:
      summary: Update a single poll choice
      description: Update a single poll choice.
      operationId: update-a-single-poll-choice
      x-api-path-slug: pollspoll-idpoll-choicesid-put
      parameters:
      - in: query
        name: poll_choices[][is_correct]
        description: Whether this poll choice is considered correct or not
      - in: query
        name: poll_choices[][position]
        description: The order this poll choice should be returned in the context
          it&#39;snsibling poll choices
      - in: query
        name: poll_choices[][text]
        description: The descriptive text of the poll choice
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Choices
      - Id
  /polls/{poll_id}/poll_sessions:
    get:
      summary: List poll sessions for a poll
      description: List poll sessions for a poll.
      operationId: list-poll-sessions-for-a-poll
      x-api-path-slug: pollspoll-idpoll-sessions-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
    post:
      summary: Create a single poll session
      description: Create a single poll session.
      operationId: create-a-single-poll-session
      x-api-path-slug: pollspoll-idpoll-sessions-post
      parameters:
      - in: query
        name: poll_sessions[][course_id]
        description: The id of the course this session is associated with
      - in: query
        name: poll_sessions[][course_section_id]
        description: The id of the course section this session is associated with
      - in: query
        name: poll_sessions[][has_public_results]
        description: Whether or not results are viewable by students
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
  /polls/{poll_id}/poll_sessions/id:
    delete:
      summary: Delete a poll session
      description: Delete a poll session.
      operationId: delete-a-poll-session
      x-api-path-slug: pollspoll-idpoll-sessionsid-delete
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
      - Id
    get:
      summary: Get the results for a single poll session
      description: Get the results for a single poll session.
      operationId: get-the-results-for-a-single-poll-session
      x-api-path-slug: pollspoll-idpoll-sessionsid-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
      - Id
    put:
      summary: Update a single poll session
      description: Update a single poll session.
      operationId: update-a-single-poll-session
      x-api-path-slug: pollspoll-idpoll-sessionsid-put
      parameters:
      - in: query
        name: poll_sessions[][course_id]
        description: The id of the course this session is associated with
      - in: query
        name: poll_sessions[][course_section_id]
        description: The id of the course section this session is associated with
      - in: query
        name: poll_sessions[][has_public_results]
        description: Whether or not results are viewable by students
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
      - Id
  /polls/{poll_id}/poll_sessions/id/close:
    get:
      summary: Close an opened poll session
      description: Close an opened poll session.
      operationId: close-an-opened-poll-session
      x-api-path-slug: pollspoll-idpoll-sessionsidclose-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
      - Id
      - Close
  /polls/{poll_id}/poll_sessions/id/open:
    get:
      summary: Open a poll session
      description: Open a poll session.
      operationId: open-a-poll-session
      x-api-path-slug: pollspoll-idpoll-sessionsidopen-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
      - Id
      - Open
  /polls/{poll_id}/poll_sessions/poll_session_id/poll_submissions:
    post:
      summary: Create a single poll submission
      description: Create a single poll submission.
      operationId: create-a-single-poll-submission
      x-api-path-slug: pollspoll-idpoll-sessionspoll-session-idpoll-submissions-post
      parameters:
      - in: query
        name: poll_submissions[][poll_choice_id]
        description: The chosen poll choice for this submission
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
      - Poll
      - Session
      - Id
      - Poll
      - Submissions
  /polls/{poll_id}/poll_sessions/poll_session_id/poll_submissions/{id}:
    get:
      summary: Get a single poll submission
      description: Get a single poll submission.
      operationId: get-a-single-poll-submission
      x-api-path-slug: pollspoll-idpoll-sessionspoll-session-idpoll-submissionsid-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
      - Poll
      - Session
      - Id
      - Poll
      - Submissions
      - Id
  /poll_sessions/closed:
    get:
      summary: List closed poll sessions
      description: List closed poll sessions.
      operationId: list-closed-poll-sessions
      x-api-path-slug: poll-sessionsclosed-get
      responses:
        200:
          description: OK
      tags:
      - Poll
      - Sessions
      - Closed
  /poll_sessions/opened:
    get:
      summary: List opened poll sessions
      description: List opened poll sessions.
      operationId: list-opened-poll-sessions
      x-api-path-slug: poll-sessionsopened-get
      responses:
        200:
          description: OK
      tags:
      - Poll
      - Sessions
      - Opened
  /quiz_submissions/{quiz_submission_id}/questions:
    get:
      summary: Get all quiz submission questions.
      description: Get all quiz submission questions..
      operationId: get-all-quiz-submission-questions
      x-api-path-slug: quiz-submissionsquiz-submission-idquestions-get
      parameters:
      - in: query
        name: include[]
        description: Associations to include with the quiz submission question
      responses:
        200:
          description: OK
      tags:
      - Quiz
      - Submissions
      - Quiz
      - Submission
      - Id
      - Questions
    post:
      summary: Answering questions
      description: Answering questions.
      operationId: answering-questions
      x-api-path-slug: quiz-submissionsquiz-submission-idquestions-post
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: attempt
        description: The attempt number of the quiz submission being taken
      - in: query
        name: quiz_questions[]
        description: Set of question IDs and the answer value
      - in: query
        name: validation_token
        description: The unique validation token you received when the Quiz Submission
          wasncreated
      responses:
        200:
          description: OK
      tags:
      - Quiz
      - Submissions
      - Quiz
      - Submission
      - Id
      - Questions
  /quiz_submissions/{quiz_submission_id}/questions/id/flag:
    put:
      summary: Flagging a question.
      description: Flagging a question..
      operationId: flagging-a-question
      x-api-path-slug: quiz-submissionsquiz-submission-idquestionsidflag-put
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: attempt
        description: The attempt number of the quiz submission being taken
      - in: query
        name: validation_token
        description: The unique validation token you received when the Quiz Submission
          wasncreated
      responses:
        200:
          description: OK
      tags:
      - Quiz
      - Submissions
      - Quiz
      - Submission
      - Id
      - Questions
      - Id
      - Flag
  /quiz_submissions/{quiz_submission_id}/questions/id/unflag:
    put:
      summary: Unflagging a question.
      description: Unflagging a question..
      operationId: unflagging-a-question
      x-api-path-slug: quiz-submissionsquiz-submission-idquestionsidunflag-put
      parameters:
      - in: query
        name: access_code
        description: Access code for the Quiz, if any
      - in: query
        name: attempt
        description: The attempt number of the quiz submission being taken
      - in: query
        name: validation_token
        description: The unique validation token you received when the Quiz Submission
          wasncreated
      responses:
        200:
          description: OK
      tags:
      - Quiz
      - Submissions
      - Quiz
      - Submission
      - Id
      - Questions
      - Id
      - Unflag
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
  /sections/{section_id}/submissions/update_grades:
    post:
      summary: Grade or comment on multiple submissions
      description: Grade or comment on multiple submissions.
      operationId: grade-or-comment-on-multiple-submissions
      x-api-path-slug: sectionssection-idsubmissionsupdate-grades-post
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
      - Submissions
      - Update
      - Grades
  /users/activity_stream:
    get:
      summary: List the activity stream
      description: List the activity stream.
      operationId: list-the-activity-stream
      x-api-path-slug: usersactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Activity
      - Stream
  /users/self/activity_stream:
    delete:
      summary: Hide all stream items
      description: Hide all stream items.
      operationId: hide-all-stream-items
      x-api-path-slug: usersselfactivity-stream-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
    get:
      summary: List the activity stream
      description: List the activity stream.
      operationId: list-the-activity-stream
      x-api-path-slug: usersselfactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
  /users/self/activity_stream/summary:
    get:
      summary: Activity stream summary
      description: Activity stream summary.
      operationId: activity-stream-summary
      x-api-path-slug: usersselfactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Summary
  /users/self/activity_stream/{id}:
    delete:
      summary: Hide a stream item
      description: Hide a stream item.
      operationId: hide-a-stream-item
      x-api-path-slug: usersselfactivity-streamid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Id
  /users/self/bookmarks:
    get:
      summary: List bookmarks
      description: List bookmarks.
      operationId: list-bookmarks
      x-api-path-slug: usersselfbookmarks-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
    post:
      summary: Create bookmark
      description: Create bookmark.
      operationId: create-bookmark
      x-api-path-slug: usersselfbookmarks-post
      parameters:
      - in: query
        name: data
        description: The data associated with the bookmark
      - in: query
        name: name
        description: The name of the bookmark
      - in: query
        name: position
        description: The position of the bookmark
      - in: query
        name: url
        description: The url of the bookmark
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
  /users/self/bookmarks/{id}:
    delete:
      summary: Delete bookmark
      description: Delete bookmark.
      operationId: delete-bookmark
      x-api-path-slug: usersselfbookmarksid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
    get:
      summary: Get bookmark
      description: Get bookmark.
      operationId: get-bookmark
      x-api-path-slug: usersselfbookmarksid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
    put:
      summary: Update bookmark
      description: Update bookmark.
      operationId: update-bookmark
      x-api-path-slug: usersselfbookmarksid-put
      parameters:
      - in: query
        name: data
        description: The data associated with the bookmark
      - in: query
        name: name
        description: The name of the bookmark
      - in: query
        name: position
        description: The position of the bookmark
      - in: query
        name: url
        description: The url of the bookmark
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
  /users/self/communication_channels/{communication_channel_id}/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
  /users/self/communication_channels/{communication_channel_id}/notification_preferences/notification:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
      - Notification
  /users/self/communication_channels/{communication_channel_id}/notification_preference_categories/category:
    put:
      summary: Update preferences by category
      description: Update preferences by category.
      operationId: update-preferences-by-category
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preference-categoriescategory-put
      parameters:
      - in: query
        name: category
        description: The name of the category
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for each notification in the category
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preference
      - Categories
      - Category
  /users/self/communication_channels/{type}/address/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
  /users/self/communication_channels/{type}/address/notification_preferences/{notification}:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
      - Notification
  /users/self/course_nicknames:
    delete:
      summary: Clear course nicknames
      description: Clear course nicknames.
      operationId: clear-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
    get:
      summary: List course nicknames
      description: List course nicknames.
      operationId: list-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
  /users/self/course_nicknames/{course_id}:
    delete:
      summary: Remove course nickname
      description: Remove course nickname.
      operationId: remove-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    get:
      summary: Get course nickname
      description: Get course nickname.
      operationId: get-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    put:
      summary: Set course nickname
      description: Set course nickname.
      operationId: set-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-put
      parameters:
      - in: query
        name: nickname
        description: The nickname to set
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
  /users/self/favorites/courses:
    delete:
      summary: Reset course favorites
      description: Reset course favorites.
      operationId: reset-course-favorites
      x-api-path-slug: usersselffavoritescourses-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
    get:
      summary: List favorite courses
      description: List favorite courses.
      operationId: list-favorite-courses
      x-api-path-slug: usersselffavoritescourses-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
  /users/self/favorites/courses/{id}:
    delete:
      summary: Remove course from favorites
      description: Remove course from favorites.
      operationId: remove-course-from-favorites
      x-api-path-slug: usersselffavoritescoursesid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the course to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
    post:
      summary: Add course to favorites
      description: Add course to favorites.
      operationId: add-course-to-favorites
      x-api-path-slug: usersselffavoritescoursesid-post
      parameters:
      - in: query
        name: id
        description: The ID or SIS ID of the course to add
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
  /users/self/favorites/groups:
    delete:
      summary: Reset group favorites
      description: Reset group favorites.
      operationId: reset-group-favorites
      x-api-path-slug: usersselffavoritesgroups-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
    get:
      summary: List favorite groups
      description: List favorite groups.
      operationId: list-favorite-groups
      x-api-path-slug: usersselffavoritesgroups-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
  /users/self/favorites/groups/{id}:
    delete:
      summary: Remove group from favorites
      description: Remove group from favorites.
      operationId: remove-group-from-favorites
      x-api-path-slug: usersselffavoritesgroupsid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the group to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
      - Id
    post:
      summary: Add group to favorites
      description: Add group to favorites.
      operationId: add-group-to-favorites
      x-api-path-slug: usersselffavoritesgroupsid-post
      parameters:
      - in: query
        name: id
        description: The ID or SIS ID of the group to add
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
      - Id
  /users/self/groups:
    get:
      summary: List your groups
      description: List your groups.
      operationId: list-your-groups
      x-api-path-slug: usersselfgroups-get
      parameters:
      - in: query
        name: context_type
        description: Only include groups that are in this type of context
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Groups
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