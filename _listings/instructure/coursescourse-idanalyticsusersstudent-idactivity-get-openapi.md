---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Get user-in-a-course-level participation data
  description: Get user-in-a-course-level participation data.
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