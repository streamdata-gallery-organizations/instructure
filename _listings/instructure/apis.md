---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: Instructure
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Appointment Groups API List appointment groups
  x-api-slug: instructure-canvas-appointment-groups-api
  description: List appointment groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups
  tags: Appointment,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groups-get-openapi.md
- name: Instructure Canvas Appointment Groups API Create an appointment group
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Create an appointment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups
  tags: Appointment,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groups-post-openapi.md
- name: Instructure Canvas Appointment Groups API Delete an appointment group
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Delete an appointment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}
  tags: Appointment,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsid-delete-openapi.md
- name: Instructure Canvas Appointment Groups API Get a single appointment group
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Get a single appointment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}
  tags: Appointment,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsid-get-openapi.md
- name: Instructure Canvas Appointment Groups API Update an appointment group
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Update an appointment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}
  tags: Appointment,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsid-put-openapi.md
- name: Instructure Canvas Appointment Groups API List student group participants
  x-api-slug: instructure-canvas-appointment-groups-api
  description: List student group participants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}/groups
  tags: Appointment,Groups,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsidgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsidgroups-get-openapi.md
- name: Instructure Canvas Appointment Groups API List user participants
  x-api-slug: instructure-canvas-appointment-groups-api
  description: List user participants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//appointment_groups/{id}/users
  tags: Appointment,Groups,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsidusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/appointment-groupsidusers-get-openapi.md
- name: Instructure Canvas Appointment Groups API
  x-api-slug: instructure-canvas-appointment-groups-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Audit API Query by account.
  x-api-slug: instructure-canvas-audit-api
  description: Query by account..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/authentication/accounts/{account_id}
  tags: Audit,Authentication,Accounts,Account,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditauthenticationaccountsaccount-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditauthenticationaccountsaccount-id-get-openapi.md
- name: Instructure Canvas Audit API Query by login.
  x-api-slug: instructure-canvas-audit-api
  description: Query by login..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/authentication/logins/{login_id}
  tags: Audit,Authentication,Logins,Login,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditauthenticationloginslogin-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditauthenticationloginslogin-id-get-openapi.md
- name: Instructure Canvas Audit API Query by user.
  x-api-slug: instructure-canvas-audit-api
  description: Query by user..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/authentication/users/{user_id}
  tags: Audit,Authentication,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditauthenticationusersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditauthenticationusersuser-id-get-openapi.md
- name: Instructure Canvas Audit API Query by course.
  x-api-slug: instructure-canvas-audit-api
  description: Query by course..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/course/courses/{course_id}
  tags: Audit,Course,Courses,Course,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditcoursecoursescourse-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditcoursecoursescourse-id-get-openapi.md
- name: Instructure Canvas Audit API Query by assignment.
  x-api-slug: instructure-canvas-audit-api
  description: Query by assignment..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/grade_change/assignments/{assignment_id}
  tags: Audit,Grade,Change,Assignments,Assignment,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditgrade-changeassignmentsassignment-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditgrade-changeassignmentsassignment-id-get-openapi.md
- name: Instructure Canvas Audit API Query by course.
  x-api-slug: instructure-canvas-audit-api
  description: Query by course..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/grade_change/courses/{course_id}
  tags: Audit,Grade,Change,Courses,Course,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditgrade-changecoursescourse-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditgrade-changecoursescourse-id-get-openapi.md
- name: Instructure Canvas Audit API Query by grader.
  x-api-slug: instructure-canvas-audit-api
  description: Query by grader..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/grade_change/graders/{grader_id}
  tags: Audit,Grade,Change,Graders,Grader,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditgrade-changegradersgrader-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditgrade-changegradersgrader-id-get-openapi.md
- name: Instructure Canvas Audit API Query by student.
  x-api-slug: instructure-canvas-audit-api
  description: Query by student..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//audit/grade_change/students/{student_id}
  tags: Audit,Grade,Change,Students,Student,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditgrade-changestudentsstudent-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/auditgrade-changestudentsstudent-id-get-openapi.md
- name: Instructure Canvas Audit API
  x-api-slug: instructure-canvas-audit-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Calendar Events API List calendar events
  x-api-slug: instructure-canvas-calendar-events-api
  description: List calendar events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events
  tags: Calendar,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-events-get-openapi.md
- name: Instructure Canvas Calendar Events API Create a calendar event
  x-api-slug: instructure-canvas-calendar-events-api
  description: Create a calendar event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events
  tags: Calendar,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-events-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-events-post-openapi.md
- name: Instructure Canvas Calendar Events API Delete a calendar event
  x-api-slug: instructure-canvas-calendar-events-api
  description: Delete a calendar event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}
  tags: Calendar,Events,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsid-delete-openapi.md
- name: Instructure Canvas Calendar Events API Get a single calendar event or assignment
  x-api-slug: instructure-canvas-calendar-events-api
  description: Get a single calendar event or assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}
  tags: Calendar,Events,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsid-get-openapi.md
- name: Instructure Canvas Calendar Events API Update a calendar event
  x-api-slug: instructure-canvas-calendar-events-api
  description: Update a calendar event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}
  tags: Calendar,Events,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsid-put-openapi.md
- name: Instructure Canvas Calendar Events API Reserve a time slot
  x-api-slug: instructure-canvas-calendar-events-api
  description: Reserve a time slot.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}/reservations
  tags: Calendar,Events,Id,Reservations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsidreservations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsidreservations-post-openapi.md
- name: Instructure Canvas Calendar Events API Reserve a time slot
  x-api-slug: instructure-canvas-calendar-events-api
  description: Reserve a time slot.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}/reservations/participant_id
  tags: Calendar,Events,Id,Reservations,Participant,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsidreservationsparticipant-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/calendar-eventsidreservationsparticipant-id-post-openapi.md
- name: Instructure Canvas Calendar Events API
  x-api-slug: instructure-canvas-calendar-events-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Conversations API List conversations
  x-api-slug: instructure-canvas-conversations-api
  description: List conversations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations
  tags: Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversations-get-openapi.md
- name: Instructure Canvas Conversations API Create a conversation
  x-api-slug: instructure-canvas-conversations-api
  description: Create a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations
  tags: Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversations-post-openapi.md
- name: Instructure Canvas Conversations API Batch update conversations
  x-api-slug: instructure-canvas-conversations-api
  description: Batch update conversations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations
  tags: Conversations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversations-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversations-put-openapi.md
- name: Instructure Canvas Conversations API Get running batches
  x-api-slug: instructure-canvas-conversations-api
  description: Get running batches.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/batches
  tags: Conversations,Batches
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsbatches-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsbatches-get-openapi.md
- name: Instructure Canvas Conversations API Find recipients
  x-api-slug: instructure-canvas-conversations-api
  description: Find recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/find_recipients
  tags: Conversations,Find,Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsfind-recipients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsfind-recipients-get-openapi.md
- name: Instructure Canvas Conversations API Mark all as read
  x-api-slug: instructure-canvas-conversations-api
  description: Mark all as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/mark_all_as_read
  tags: Conversations,Mark,,As,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsmark-all-as-read-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsmark-all-as-read-post-openapi.md
- name: Instructure Canvas Conversations API Unread count
  x-api-slug: instructure-canvas-conversations-api
  description: Unread count.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/unread_count
  tags: Conversations,Unread,Count
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsunread-count-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsunread-count-get-openapi.md
- name: Instructure Canvas Conversations API Delete a conversation
  x-api-slug: instructure-canvas-conversations-api
  description: Delete a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}
  tags: Conversations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsid-delete-openapi.md
- name: Instructure Canvas Conversations API Get a single conversation
  x-api-slug: instructure-canvas-conversations-api
  description: Get a single conversation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}
  tags: Conversations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsid-get-openapi.md
- name: Instructure Canvas Conversations API Edit a conversation
  x-api-slug: instructure-canvas-conversations-api
  description: Edit a conversation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}
  tags: Conversations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsid-put-openapi.md
- name: Instructure Canvas Conversations API Add a message
  x-api-slug: instructure-canvas-conversations-api
  description: Add a message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}/add_message
  tags: Conversations,Id,Add,Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsidadd-message-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsidadd-message-post-openapi.md
- name: Instructure Canvas Conversations API Add recipients
  x-api-slug: instructure-canvas-conversations-api
  description: Add recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}/add_recipients
  tags: Conversations,Id,Add,Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsidadd-recipients-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsidadd-recipients-post-openapi.md
- name: Instructure Canvas Conversations API Delete a message
  x-api-slug: instructure-canvas-conversations-api
  description: Delete a message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//conversations/{id}/remove_messages
  tags: Conversations,Id,Remove,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsidremove-messages-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/conversationsidremove-messages-post-openapi.md
- name: Instructure Canvas Conversations API
  x-api-slug: instructure-canvas-conversations-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Courses API List your courses
  x-api-slug: instructure-canvas-courses-api
  description: List your courses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses
  tags: Courses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/courses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/courses-get-openapi.md
- name: Instructure Canvas Courses API Course activity stream
  x-api-slug: instructure-canvas-courses-api
  description: Course activity stream.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/activity_stream
  tags: Courses,Course,Id,Activity,Stream
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idactivity-stream-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idactivity-stream-get-openapi.md
- name: Instructure Canvas Courses API Course activity stream summary
  x-api-slug: instructure-canvas-courses-api
  description: Course activity stream summary.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/activity_stream/summary
  tags: Courses,Course,Id,Activity,Stream,Summary
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idactivity-streamsummary-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idactivity-streamsummary-get-openapi.md
- name: Instructure Canvas Courses API Get course-level participation data
  x-api-slug: instructure-canvas-courses-api
  description: Get course-level participation data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/activity
  tags: Courses,Course,Id,Analytics,Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsactivity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsactivity-get-openapi.md
- name: Instructure Canvas Courses API Get course-level assignment data
  x-api-slug: instructure-canvas-courses-api
  description: Get course-level assignment data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/assignments
  tags: Courses,Course,Id,Analytics,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsassignments-get-openapi.md
- name: Instructure Canvas Courses API Get course-level student summary data
  x-api-slug: instructure-canvas-courses-api
  description: Get course-level student summary data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/student_summaries
  tags: Courses,Course,Id,Analytics,Student,Summaries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsstudent-summaries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsstudent-summaries-get-openapi.md
- name: Instructure Canvas Courses API Get user-in-a-course-level participation data
  x-api-slug: instructure-canvas-courses-api
  description: Get user-in-a-course-level participation data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/users/student_id/activity
  tags: Courses,Course,Id,Analytics,Users,Student,Id,Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idactivity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idactivity-get-openapi.md
- name: Instructure Canvas Courses API Get user-in-a-course-level assignment data
  x-api-slug: instructure-canvas-courses-api
  description: Get user-in-a-course-level assignment data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/users/student_id/assignments
  tags: Courses,Course,Id,Analytics,Users,Student,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idassignments-get-openapi.md
- name: Instructure Canvas Courses API Get user-in-a-course-level messaging data
  x-api-slug: instructure-canvas-courses-api
  description: Get user-in-a-course-level messaging data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/analytics/users/student_id/communication
  tags: Courses,Course,Id,Analytics,Users,Student,Id,Communication
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idcommunication-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idanalyticsusersstudent-idcommunication-get-openapi.md
- name: Instructure Canvas Courses API List assignments
  x-api-slug: instructure-canvas-courses-api
  description: List assignments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments
  tags: Courses,Course,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignments-get-openapi.md
- name: Instructure Canvas Courses API Create an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Create an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments
  tags: Courses,Course,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignments-post-openapi.md
- name: Instructure Canvas Courses API List gradeable students
  x-api-slug: instructure-canvas-courses-api
  description: List gradeable students.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/gradeable_students
  tags: Courses,Course,Id,Assignments,Assignment,Id,Gradeable,Students
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idgradeable-students-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idgradeable-students-get-openapi.md
- name: Instructure Canvas Courses API List students selected for moderation
  x-api-slug: instructure-canvas-courses-api
  description: List students selected for moderation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/moderated_students
  tags: Courses,Course,Id,Assignments,Assignment,Id,Moderated,Students
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idmoderated-students-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idmoderated-students-get-openapi.md
- name: Instructure Canvas Courses API Select students for moderation
  x-api-slug: instructure-canvas-courses-api
  description: Select students for moderation.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/moderated_students
  tags: Courses,Course,Id,Assignments,Assignment,Id,Moderated,Students
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idmoderated-students-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idmoderated-students-post-openapi.md
- name: Instructure Canvas Courses API List assignment overrides
  x-api-slug: instructure-canvas-courses-api
  description: List assignment overrides.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverrides-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverrides-get-openapi.md
- name: Instructure Canvas Courses API Create an assignment override
  x-api-slug: instructure-canvas-courses-api
  description: Create an assignment override.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverrides-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverrides-post-openapi.md
- name: Instructure Canvas Courses API Delete an assignment override
  x-api-slug: instructure-canvas-courses-api
  description: Delete an assignment override.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides/{id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single assignment override
  x-api-slug: instructure-canvas-courses-api
  description: Get a single assignment override.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides/{id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-get-openapi.md
- name: Instructure Canvas Courses API Update an assignment override
  x-api-slug: instructure-canvas-courses-api
  description: Update an assignment override.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/overrides/{id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Overrides,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idoverridesid-put-openapi.md
- name: Instructure Canvas Courses API Get all Peer Reviews
  x-api-slug: instructure-canvas-courses-api
  description: Get all peer reviews.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/peer_reviews
  tags: Courses,Course,Id,Assignments,Assignment,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idpeer-reviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idpeer-reviews-get-openapi.md
- name: Instructure Canvas Courses API Publish provisional grades for an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Publish provisional grades for an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/provisional_grades/publish
  tags: Courses,Course,Id,Assignments,Assignment,Id,Provisional,Grades,Publish
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradespublish-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradespublish-post-openapi.md
- name: Instructure Canvas Courses API Show provisional grade status for a student
  x-api-slug: instructure-canvas-courses-api
  description: Show provisional grade status for a student.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/provisional_grades/status
  tags: Courses,Course,Id,Assignments,Assignment,Id,Provisional,Grades,Status
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesstatus-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesstatus-get-openapi.md
- name: Instructure Canvas Courses API Copy provisional grade
  x-api-slug: instructure-canvas-courses-api
  description: Copy provisional grade.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/provisional_grades/{provisional_grade_id}/copy_to_final_mark
  tags: Courses,Course,Id,Assignments,Assignment,Id,Provisional,Grades,Provisional,Grade,Id,Copy,To,Final,Mark
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idcopy-to-final-mark-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idcopy-to-final-mark-post-openapi.md
- name: Instructure Canvas Courses API Select provisional grade
  x-api-slug: instructure-canvas-courses-api
  description: Select provisional grade.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/provisional_grades/{provisional_grade_id}/select
  tags: Courses,Course,Id,Assignments,Assignment,Id,Provisional,Grades,Provisional,Grade,Id,Select
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idselect-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idprovisional-gradesprovisional-grade-idselect-put-openapi.md
- name: Instructure Canvas Courses API List assignment submissions
  x-api-slug: instructure-canvas-courses-api
  description: List assignment submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissions-get-openapi.md
- name: Instructure Canvas Courses API Submit an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Submit an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissions-post-openapi.md
- name: Instructure Canvas Courses API Grade or comment on multiple submissions
  x-api-slug: instructure-canvas-courses-api
  description: Grade or comment on multiple submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/update_grades
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,Update,Grades
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsupdate-grades-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsupdate-grades-post-openapi.md
- name: Instructure Canvas Courses API Create Peer Review
  x-api-slug: instructure-canvas-courses-api
  description: Create peer review.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete-openapi.md
- name: Instructure Canvas Courses API Get all Peer Reviews
  x-api-slug: instructure-canvas-courses-api
  description: Get all peer reviews.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get-openapi.md
- name: Instructure Canvas Courses API Create Peer Review
  x-api-slug: instructure-canvas-courses-api
  description: Create peer review.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post-openapi.md
- name: Instructure Canvas Courses API Get a single submission
  x-api-slug: instructure-canvas-courses-api
  description: Get a single submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-id-get-openapi.md
- name: Instructure Canvas Courses API Grade or comment on a submission
  x-api-slug: instructure-canvas-courses-api
  description: Grade or comment on a submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-id-put-openapi.md
- name: Instructure Canvas Courses API Upload a file
  x-api-slug: instructure-canvas-courses-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}/comments/files
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id,Comments,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idcommentsfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idcommentsfiles-post-openapi.md
- name: Instructure Canvas Courses API Upload a file
  x-api-slug: instructure-canvas-courses-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}/files
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idfiles-post-openapi.md
- name: Instructure Canvas Courses API Mark submission as unread
  x-api-slug: instructure-canvas-courses-api
  description: Mark submission as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}/read
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idread-delete-openapi.md
- name: Instructure Canvas Courses API Mark submission as read
  x-api-slug: instructure-canvas-courses-api
  description: Mark submission as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/assignment_id/submissions/{user_id}/read
  tags: Courses,Course,Id,Assignments,Assignment,Id,Submissions,User,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsassignment-idsubmissionsuser-idread-put-openapi.md
- name: Instructure Canvas Courses API Delete an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Delete an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/id
  tags: Courses,Course,Id,Assignments,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single assignment
  x-api-slug: instructure-canvas-courses-api
  description: Get a single assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/id
  tags: Courses,Course,Id,Assignments,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsid-get-openapi.md
- name: Instructure Canvas Courses API Edit an assignment
  x-api-slug: instructure-canvas-courses-api
  description: Edit an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignments/id
  tags: Courses,Course,Id,Assignments,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignmentsid-put-openapi.md
- name: Instructure Canvas Courses API List assignment groups
  x-api-slug: instructure-canvas-courses-api
  description: List assignment groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups
  tags: Courses,Course,Id,Assignment,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groups-get-openapi.md
- name: Instructure Canvas Courses API Create an Assignment Group
  x-api-slug: instructure-canvas-courses-api
  description: Create an assignment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups
  tags: Courses,Course,Id,Assignment,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groups-post-openapi.md
- name: Instructure Canvas Courses API Destroy an Assignment Group
  x-api-slug: instructure-canvas-courses-api
  description: Destroy an assignment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups/assignment_group_id
  tags: Courses,Course,Id,Assignment,Groups,Assignment,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-delete-openapi.md
- name: Instructure Canvas Courses API Get an Assignment Group
  x-api-slug: instructure-canvas-courses-api
  description: Get an assignment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups/assignment_group_id
  tags: Courses,Course,Id,Assignment,Groups,Assignment,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-get-openapi.md
- name: Instructure Canvas Courses API Edit an Assignment Group
  x-api-slug: instructure-canvas-courses-api
  description: Edit an assignment group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/assignment_groups/assignment_group_id
  tags: Courses,Course,Id,Assignment,Groups,Assignment,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idassignment-groupsassignment-group-id-put-openapi.md
- name: Instructure Canvas Courses API List conferences
  x-api-slug: instructure-canvas-courses-api
  description: List conferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/conferences
  tags: Courses,Course,Id,Conferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idconferences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idconferences-get-openapi.md
- name: Instructure Canvas Courses API List content exports
  x-api-slug: instructure-canvas-courses-api
  description: List content exports.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_exports
  tags: Courses,Course,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-exports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-exports-get-openapi.md
- name: Instructure Canvas Courses API Export content
  x-api-slug: instructure-canvas-courses-api
  description: Export content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_exports
  tags: Courses,Course,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-exports-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-exports-post-openapi.md
- name: Instructure Canvas Courses API Show content export
  x-api-slug: instructure-canvas-courses-api
  description: Show content export.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_exports/id
  tags: Courses,Course,Id,Content,Exports,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-exportsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-exportsid-get-openapi.md
- name: Instructure Canvas Courses API List licenses
  x-api-slug: instructure-canvas-courses-api
  description: List licenses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_licenses
  tags: Courses,Course,Id,Content,Licenses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-licenses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-licenses-get-openapi.md
- name: Instructure Canvas Courses API List content migrations
  x-api-slug: instructure-canvas-courses-api
  description: List content migrations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_migrations
  tags: Courses,Course,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrations-get-openapi.md
- name: Instructure Canvas Courses API Create a content migration
  x-api-slug: instructure-canvas-courses-api
  description: Create a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_migrations
  tags: Courses,Course,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrations-post-openapi.md
- name: Instructure Canvas Courses API List migration issues
  x-api-slug: instructure-canvas-courses-api
  description: List migration issues.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_migrations/content_migration_id/migration_issues
  tags: Courses,Course,Id,Content,Migrations,Content,Migration,Id,Migration,Issues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationscontent-migration-idmigration-issues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationscontent-migration-idmigration-issues-get-openapi.md
- name: Instructure Canvas Courses API Get a migration issue
  x-api-slug: instructure-canvas-courses-api
  description: Get a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Courses,Course,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationscontent-migration-idmigration-issuesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationscontent-migration-idmigration-issuesid-get-openapi.md
- name: Instructure Canvas Courses API Update a migration issue
  x-api-slug: instructure-canvas-courses-api
  description: Update a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Courses,Course,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationscontent-migration-idmigration-issuesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationscontent-migration-idmigration-issuesid-put-openapi.md
- name: Instructure Canvas Courses API Get a content migration
  x-api-slug: instructure-canvas-courses-api
  description: Get a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_migrations/id
  tags: Courses,Course,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationsid-get-openapi.md
- name: Instructure Canvas Courses API Update a content migration
  x-api-slug: instructure-canvas-courses-api
  description: Update a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_migrations/id
  tags: Courses,Course,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationsid-put-openapi.md
- name: Instructure Canvas Courses API List Migration Systems
  x-api-slug: instructure-canvas-courses-api
  description: List migration systems.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/content_migrations/migrators
  tags: Courses,Course,Id,Content,Migrations,Migrators
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationsmigrators-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcontent-migrationsmigrators-get-openapi.md
- name: Instructure Canvas Courses API Copy course content
  x-api-slug: instructure-canvas-courses-api
  description: Copy course content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/course_copy
  tags: Courses,Course,Id,Course,Copy
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcourse-copy-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcourse-copy-post-openapi.md
- name: Instructure Canvas Courses API Get course copy status
  x-api-slug: instructure-canvas-courses-api
  description: Get course copy status.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/course_copy/id
  tags: Courses,Course,Id,Course,Copy,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcourse-copyid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcourse-copyid-get-openapi.md
- name: Instructure Canvas Courses API List custom gradebook columns
  x-api-slug: instructure-canvas-courses-api
  description: List custom gradebook columns.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/custom_gradebook_columns
  tags: Courses,Course,Id,Custom,Gradebook,Columns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columns-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columns-get-openapi.md
- name: Instructure Canvas Courses API Create a custom gradebook column
  x-api-slug: instructure-canvas-courses-api
  description: Create a custom gradebook column.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/custom_gradebook_columns
  tags: Courses,Course,Id,Custom,Gradebook,Columns
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columns-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columns-post-openapi.md
- name: Instructure Canvas Courses API Delete a custom gradebook column
  x-api-slug: instructure-canvas-courses-api
  description: Delete a custom gradebook column.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/custom_gradebook_columns/id
  tags: Courses,Course,Id,Custom,Gradebook,Columns,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsid-delete-openapi.md
- name: Instructure Canvas Courses API Update a custom gradebook column
  x-api-slug: instructure-canvas-courses-api
  description: Update a custom gradebook column.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/custom_gradebook_columns/id
  tags: Courses,Course,Id,Custom,Gradebook,Columns,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsid-put-openapi.md
- name: Instructure Canvas Courses API List entries for a column
  x-api-slug: instructure-canvas-courses-api
  description: List entries for a column.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/custom_gradebook_columns/id/data
  tags: Courses,Course,Id,Custom,Gradebook,Columns,Id,Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsiddata-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsiddata-get-openapi.md
- name: Instructure Canvas Courses API Update column data
  x-api-slug: instructure-canvas-courses-api
  description: Update column data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/custom_gradebook_columns/id/data/{user_id}
  tags: Courses,Course,Id,Custom,Gradebook,Columns,Id,Data,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsiddatauser-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsiddatauser-id-put-openapi.md
- name: Instructure Canvas Courses API Reorder custom columns
  x-api-slug: instructure-canvas-courses-api
  description: Reorder custom columns.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/custom_gradebook_columns/reorder
  tags: Courses,Course,Id,Custom,Gradebook,Columns,Reorder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsreorder-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idcustom-gradebook-columnsreorder-post-openapi.md
- name: Instructure Canvas Courses API List discussion topics
  x-api-slug: instructure-canvas-courses-api
  description: List discussion topics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics
  tags: Courses,Course,Id,Discussion,Topics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topics-get-openapi.md
- name: Instructure Canvas Courses API Create a new discussion topic
  x-api-slug: instructure-canvas-courses-api
  description: Create a new discussion topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics
  tags: Courses,Course,Id,Discussion,Topics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topics-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topics-post-openapi.md
- name: Instructure Canvas Courses API Reorder pinned topics
  x-api-slug: instructure-canvas-courses-api
  description: Reorder pinned topics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/reorder
  tags: Courses,Course,Id,Discussion,Topics,Reorder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicsreorder-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicsreorder-post-openapi.md
- name: Instructure Canvas Courses API Delete a topic
  x-api-slug: instructure-canvas-courses-api
  description: Delete a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-id-delete-openapi.md
- name: Instructure Canvas Courses API Get a single topic
  x-api-slug: instructure-canvas-courses-api
  description: Get a single topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-id-get-openapi.md
- name: Instructure Canvas Courses API Update a topic
  x-api-slug: instructure-canvas-courses-api
  description: Update a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-id-put-openapi.md
- name: Instructure Canvas Courses API List topic entries
  x-api-slug: instructure-canvas-courses-api
  description: List topic entries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entries
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identries-get-openapi.md
- name: Instructure Canvas Courses API Post an entry
  x-api-slug: instructure-canvas-courses-api
  description: Post an entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entries
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identries-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identries-post-openapi.md
- name: Instructure Canvas Courses API Rate entry
  x-api-slug: instructure-canvas-courses-api
  description: Rate entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entries/{entry_id}/rating
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Rating
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idrating-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idrating-post-openapi.md
- name: Instructure Canvas Courses API Mark entry as unread
  x-api-slug: instructure-canvas-courses-api
  description: Mark entry as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entries/{entry_id}/read
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idread-delete-openapi.md
- name: Instructure Canvas Courses API Mark entry as read
  x-api-slug: instructure-canvas-courses-api
  description: Mark entry as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entries/{entry_id}/read
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idread-put-openapi.md
- name: Instructure Canvas Courses API List entry replies
  x-api-slug: instructure-canvas-courses-api
  description: List entry replies.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entries/{entry_id}/replies
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Replies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idreplies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idreplies-get-openapi.md
- name: Instructure Canvas Courses API Post a reply
  x-api-slug: instructure-canvas-courses-api
  description: Post a reply.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entries/{entry_id}/replies
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Replies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idreplies-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesentry-idreplies-post-openapi.md
- name: Instructure Canvas Courses API Delete an entry
  x-api-slug: instructure-canvas-courses-api
  description: Delete an entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entries/{id}
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entries,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesid-delete-openapi.md
- name: Instructure Canvas Courses API Update an entry
  x-api-slug: instructure-canvas-courses-api
  description: Update an entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entries/{id}
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entries,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identriesid-put-openapi.md
- name: Instructure Canvas Courses API List entries
  x-api-slug: instructure-canvas-courses-api
  description: List entries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/entry_list
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Entry,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identry-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-identry-list-get-openapi.md
- name: Instructure Canvas Courses API Mark topic as unread
  x-api-slug: instructure-canvas-courses-api
  description: Mark topic as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/read
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idread-delete-openapi.md
- name: Instructure Canvas Courses API Mark topic as read
  x-api-slug: instructure-canvas-courses-api
  description: Mark topic as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/read
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idread-put-openapi.md
- name: Instructure Canvas Courses API Mark all entries as unread
  x-api-slug: instructure-canvas-courses-api
  description: Mark all entries as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/read_all
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idread-all-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idread-all-delete-openapi.md
- name: Instructure Canvas Courses API Mark all entries as read
  x-api-slug: instructure-canvas-courses-api
  description: Mark all entries as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/read_all
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idread-all-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idread-all-put-openapi.md
- name: Instructure Canvas Courses API Unsubscribe from a topic
  x-api-slug: instructure-canvas-courses-api
  description: Unsubscribe from a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/subscribed
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Subscribed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idsubscribed-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idsubscribed-delete-openapi.md
- name: Instructure Canvas Courses API Subscribe to a topic
  x-api-slug: instructure-canvas-courses-api
  description: Subscribe to a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/subscribed
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,Subscribed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idsubscribed-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idsubscribed-put-openapi.md
- name: Instructure Canvas Courses API Get the full topic
  x-api-slug: instructure-canvas-courses-api
  description: Get the full topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/discussion_topics/topic_id/view
  tags: Courses,Course,Id,Discussion,Topics,Topic,Id,View
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idview-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-iddiscussion-topicstopic-idview-get-openapi.md
- name: Instructure Canvas Courses API List enrollments
  x-api-slug: instructure-canvas-courses-api
  description: List enrollments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/enrollments
  tags: Courses,Course,Id,Enrollments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idenrollments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idenrollments-get-openapi.md
- name: Instructure Canvas Courses API Enroll a user
  x-api-slug: instructure-canvas-courses-api
  description: Enroll a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/enrollments
  tags: Courses,Course,Id,Enrollments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idenrollments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idenrollments-post-openapi.md
- name: Instructure Canvas Courses API Conclude or inactivate an enrollment
  x-api-slug: instructure-canvas-courses-api
  description: Conclude or inactivate an enrollment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/enrollments/id
  tags: Courses,Course,Id,Enrollments,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idenrollmentsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idenrollmentsid-delete-openapi.md
- name: Instructure Canvas Courses API Re-activate an enrollment
  x-api-slug: instructure-canvas-courses-api
  description: Re-activate an enrollment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/enrollments/id/reactivate
  tags: Courses,Course,Id,Enrollments,Id,Reactivate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idenrollmentsidreactivate-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idenrollmentsidreactivate-put-openapi.md
- name: Instructure Canvas Courses API Show ePub export
  x-api-slug: instructure-canvas-courses-api
  description: Show epub export.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/epub_exports/id
  tags: Courses,Course,Id,Epub,Exports,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idepub-exportsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idepub-exportsid-get-openapi.md
- name: Instructure Canvas Courses API List external feeds
  x-api-slug: instructure-canvas-courses-api
  description: List external feeds.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/external_feeds
  tags: Courses,Course,Id,External,Feeds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-feeds-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-feeds-get-openapi.md
- name: Instructure Canvas Courses API Create an external feed
  x-api-slug: instructure-canvas-courses-api
  description: Create an external feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/external_feeds
  tags: Courses,Course,Id,External,Feeds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-feeds-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-feeds-post-openapi.md
- name: Instructure Canvas Courses API Delete an external feed
  x-api-slug: instructure-canvas-courses-api
  description: Delete an external feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/external_feeds/external_feed_id
  tags: Courses,Course,Id,External,Feeds,External,Feed,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-feedsexternal-feed-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-feedsexternal-feed-id-delete-openapi.md
- name: Instructure Canvas Courses API List external tools
  x-api-slug: instructure-canvas-courses-api
  description: List external tools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/external_tools
  tags: Courses,Course,Id,External,Tools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-tools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-tools-get-openapi.md
- name: Instructure Canvas Courses API Create an external tool
  x-api-slug: instructure-canvas-courses-api
  description: Create an external tool.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/external_tools
  tags: Courses,Course,Id,External,Tools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-tools-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-tools-post-openapi.md
- name: Instructure Canvas Courses API Delete an external tool
  x-api-slug: instructure-canvas-courses-api
  description: Delete an external tool.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/external_tools/external_tool_id
  tags: Courses,Course,Id,External,Tools,External,Tool,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-toolsexternal-tool-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-toolsexternal-tool-id-delete-openapi.md
- name: Instructure Canvas Courses API Get a single external tool
  x-api-slug: instructure-canvas-courses-api
  description: Get a single external tool.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/external_tools/external_tool_id
  tags: Courses,Course,Id,External,Tools,External,Tool,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-toolsexternal-tool-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-toolsexternal-tool-id-get-openapi.md
- name: Instructure Canvas Courses API Edit an external tool
  x-api-slug: instructure-canvas-courses-api
  description: Edit an external tool.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/external_tools/external_tool_id
  tags: Courses,Course,Id,External,Tools,External,Tool,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-toolsexternal-tool-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-toolsexternal-tool-id-put-openapi.md
- name: Instructure Canvas Courses API Get a sessionless launch url for an external
    tool.
  x-api-slug: instructure-canvas-courses-api
  description: Get a sessionless launch url for an external tool..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/external_tools/sessionless_launch
  tags: Courses,Course,Id,External,Tools,Sessionless,Launch
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-toolssessionless-launch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idexternal-toolssessionless-launch-get-openapi.md
- name: Instructure Canvas Courses API List features
  x-api-slug: instructure-canvas-courses-api
  description: List features.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/features
  tags: Courses,Course,Id,Features
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeatures-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeatures-get-openapi.md
- name: Instructure Canvas Courses API List enabled features
  x-api-slug: instructure-canvas-courses-api
  description: List enabled features.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/features/enabled
  tags: Courses,Course,Id,Features,Enabled
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeaturesenabled-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeaturesenabled-get-openapi.md
- name: Instructure Canvas Courses API Remove feature flag
  x-api-slug: instructure-canvas-courses-api
  description: Remove feature flag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/features/flags/feature
  tags: Courses,Course,Id,Features,Flags,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeaturesflagsfeature-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeaturesflagsfeature-delete-openapi.md
- name: Instructure Canvas Courses API Get feature flag
  x-api-slug: instructure-canvas-courses-api
  description: Get feature flag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/features/flags/feature
  tags: Courses,Course,Id,Features,Flags,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeaturesflagsfeature-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeaturesflagsfeature-get-openapi.md
- name: Instructure Canvas Courses API Set feature flag
  x-api-slug: instructure-canvas-courses-api
  description: Set feature flag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/features/flags/feature
  tags: Courses,Course,Id,Features,Flags,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeaturesflagsfeature-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfeaturesflagsfeature-put-openapi.md
- name: Instructure Canvas Courses API List files
  x-api-slug: instructure-canvas-courses-api
  description: List files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/files
  tags: Courses,Course,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfiles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfiles-get-openapi.md
- name: Instructure Canvas Courses API Upload a file
  x-api-slug: instructure-canvas-courses-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/files
  tags: Courses,Course,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfiles-post-openapi.md
- name: Instructure Canvas Courses API Get file
  x-api-slug: instructure-canvas-courses-api
  description: Get file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/files/id
  tags: Courses,Course,Id,Files,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfilesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfilesid-get-openapi.md
- name: Instructure Canvas Courses API Get quota information
  x-api-slug: instructure-canvas-courses-api
  description: Get quota information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/files/quota
  tags: Courses,Course,Id,Files,Quota
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfilesquota-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfilesquota-get-openapi.md
- name: Instructure Canvas Courses API List all folders
  x-api-slug: instructure-canvas-courses-api
  description: List all folders.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/folders
  tags: Courses,Course,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfolders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfolders-get-openapi.md
- name: Instructure Canvas Courses API Create folder
  x-api-slug: instructure-canvas-courses-api
  description: Create folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/folders
  tags: Courses,Course,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfolders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfolders-post-openapi.md
- name: Instructure Canvas Courses API Resolve path
  x-api-slug: instructure-canvas-courses-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/folders/by_path
  tags: Courses,Course,Id,Folders,By,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfoldersby-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfoldersby-path-get-openapi.md
- name: Instructure Canvas Courses API Resolve path
  x-api-slug: instructure-canvas-courses-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/folders/by_path/*full_path
  tags: Courses,Course,Id,Folders,By,Path,*full,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfoldersby-pathfull-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfoldersby-pathfull-path-get-openapi.md
- name: Instructure Canvas Courses API Get folder
  x-api-slug: instructure-canvas-courses-api
  description: Get folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/folders/id
  tags: Courses,Course,Id,Folders,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfoldersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfoldersid-get-openapi.md
- name: Instructure Canvas Courses API Show front page
  x-api-slug: instructure-canvas-courses-api
  description: Show front page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/front_page
  tags: Courses,Course,Id,Front,Page
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfront-page-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfront-page-get-openapi.md
- name: Instructure Canvas Courses API Update/create front page
  x-api-slug: instructure-canvas-courses-api
  description: Update/create front page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/front_page
  tags: Courses,Course,Id,Front,Page
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfront-page-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idfront-page-put-openapi.md
- name: Instructure Canvas Courses API Details for a given date in gradebook history
    for this course
  x-api-slug: instructure-canvas-courses-api
  description: Details for a given date in gradebook history for this course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/gradebook_history/date
  tags: Courses,Course,Id,Gradebook,History,Date
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgradebook-historydate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgradebook-historydate-get-openapi.md
- name: Instructure Canvas Courses API Lists submissions
  x-api-slug: instructure-canvas-courses-api
  description: Lists submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/gradebook_history/date/graders/{grader_id}/assignments/assignment_id/submissions
  tags: Courses,Course,Id,Gradebook,History,Date,Graders,Grader,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgradebook-historydategradersgrader-idassignmentsassignment-idsubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgradebook-historydategradersgrader-idassignmentsassignment-idsubmissions-get-openapi.md
- name: Instructure Canvas Courses API Days in gradebook history for this course
  x-api-slug: instructure-canvas-courses-api
  description: Days in gradebook history for this course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/gradebook_history/days
  tags: Courses,Course,Id,Gradebook,History,Days
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgradebook-historydays-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgradebook-historydays-get-openapi.md
- name: Instructure Canvas Courses API List uncollated submission versions
  x-api-slug: instructure-canvas-courses-api
  description: List uncollated submission versions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/gradebook_history/feed
  tags: Courses,Course,Id,Gradebook,History,Feed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgradebook-historyfeed-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgradebook-historyfeed-get-openapi.md
- name: Instructure Canvas Courses API List grading periods
  x-api-slug: instructure-canvas-courses-api
  description: List grading periods.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/grading_periods
  tags: Courses,Course,Id,Grading,Periods
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periods-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periods-get-openapi.md
- name: Instructure Canvas Courses API Create a single grading period
  x-api-slug: instructure-canvas-courses-api
  description: Create a single grading period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/grading_periods
  tags: Courses,Course,Id,Grading,Periods
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periods-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periods-post-openapi.md
- name: Instructure Canvas Courses API Delete a grading period
  x-api-slug: instructure-canvas-courses-api
  description: Delete a grading period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/grading_periods/id
  tags: Courses,Course,Id,Grading,Periods,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periodsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periodsid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single grading period
  x-api-slug: instructure-canvas-courses-api
  description: Get a single grading period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/grading_periods/id
  tags: Courses,Course,Id,Grading,Periods,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periodsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periodsid-get-openapi.md
- name: Instructure Canvas Courses API Update a single grading period
  x-api-slug: instructure-canvas-courses-api
  description: Update a single grading period.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/grading_periods/id
  tags: Courses,Course,Id,Grading,Periods,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periodsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-periodsid-put-openapi.md
- name: Instructure Canvas Courses API List the grading standards available in a context.
  x-api-slug: instructure-canvas-courses-api
  description: List the grading standards available in a context..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/grading_standards
  tags: Courses,Course,Id,Grading,Standards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-standards-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-standards-get-openapi.md
- name: Instructure Canvas Courses API Create a new grading standard
  x-api-slug: instructure-canvas-courses-api
  description: Create a new grading standard.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/grading_standards
  tags: Courses,Course,Id,Grading,Standards
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-standards-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgrading-standards-post-openapi.md
- name: Instructure Canvas Courses API List the groups available in a context.
  x-api-slug: instructure-canvas-courses-api
  description: List the groups available in a context..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/groups
  tags: Courses,Course,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgroups-get-openapi.md
- name: Instructure Canvas Courses API List group categories for a context
  x-api-slug: instructure-canvas-courses-api
  description: List group categories for a context.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/group_categories
  tags: Courses,Course,Id,Group,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgroup-categories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgroup-categories-get-openapi.md
- name: Instructure Canvas Courses API Create a Group Category
  x-api-slug: instructure-canvas-courses-api
  description: Create a group category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/group_categories
  tags: Courses,Course,Id,Group,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgroup-categories-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idgroup-categories-post-openapi.md
- name: Instructure Canvas Courses API List live assessments
  x-api-slug: instructure-canvas-courses-api
  description: List live assessments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/live_assessments
  tags: Courses,Course,Id,Live,Assessments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idlive-assessments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idlive-assessments-get-openapi.md
- name: Instructure Canvas Courses API Create or find a live assessment
  x-api-slug: instructure-canvas-courses-api
  description: Create or find a live assessment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/live_assessments
  tags: Courses,Course,Id,Live,Assessments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idlive-assessments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idlive-assessments-post-openapi.md
- name: Instructure Canvas Courses API List live assessment results
  x-api-slug: instructure-canvas-courses-api
  description: List live assessment results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/live_assessments/assessment_id/results
  tags: Courses,Course,Id,Live,Assessments,Assessment,Id,Results
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idlive-assessmentsassessment-idresults-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idlive-assessmentsassessment-idresults-get-openapi.md
- name: Instructure Canvas Courses API Create live assessment results
  x-api-slug: instructure-canvas-courses-api
  description: Create live assessment results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/live_assessments/assessment_id/results
  tags: Courses,Course,Id,Live,Assessments,Assessment,Id,Results
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idlive-assessmentsassessment-idresults-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idlive-assessmentsassessment-idresults-post-openapi.md
- name: Instructure Canvas Courses API List modules
  x-api-slug: instructure-canvas-courses-api
  description: List modules.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules
  tags: Courses,Course,Id,Modules
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodules-get-openapi.md
- name: Instructure Canvas Courses API Create a module
  x-api-slug: instructure-canvas-courses-api
  description: Create a module.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules
  tags: Courses,Course,Id,Modules
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodules-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodules-post-openapi.md
- name: Instructure Canvas Courses API Delete module
  x-api-slug: instructure-canvas-courses-api
  description: Delete module.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/id
  tags: Courses,Course,Id,Modules,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesid-delete-openapi.md
- name: Instructure Canvas Courses API Show module
  x-api-slug: instructure-canvas-courses-api
  description: Show module.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/id
  tags: Courses,Course,Id,Modules,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesid-get-openapi.md
- name: Instructure Canvas Courses API Update a module
  x-api-slug: instructure-canvas-courses-api
  description: Update a module.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/id
  tags: Courses,Course,Id,Modules,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesid-put-openapi.md
- name: Instructure Canvas Courses API Re-lock module progressions
  x-api-slug: instructure-canvas-courses-api
  description: Re-lock module progressions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/id/relock
  tags: Courses,Course,Id,Modules,Id,Relock
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesidrelock-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesidrelock-put-openapi.md
- name: Instructure Canvas Courses API List module items
  x-api-slug: instructure-canvas-courses-api
  description: List module items.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items
  tags: Courses,Course,Id,Modules,Module,Id,Items
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditems-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditems-get-openapi.md
- name: Instructure Canvas Courses API Create a module item
  x-api-slug: instructure-canvas-courses-api
  description: Create a module item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items
  tags: Courses,Course,Id,Modules,Module,Id,Items
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditems-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditems-post-openapi.md
- name: Instructure Canvas Courses API Delete module item
  x-api-slug: instructure-canvas-courses-api
  description: Delete module item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-delete-openapi.md
- name: Instructure Canvas Courses API Show module item
  x-api-slug: instructure-canvas-courses-api
  description: Show module item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-get-openapi.md
- name: Instructure Canvas Courses API Update a module item
  x-api-slug: instructure-canvas-courses-api
  description: Update a module item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsid-put-openapi.md
- name: Instructure Canvas Courses API Mark module item as done/not done
  x-api-slug: instructure-canvas-courses-api
  description: Mark module item as done/not done.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}/done
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id,Done
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsiddone-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsiddone-put-openapi.md
- name: Instructure Canvas Courses API Mark module item read
  x-api-slug: instructure-canvas-courses-api
  description: Mark module item read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/modules/module_id/items/{id}/mark_read
  tags: Courses,Course,Id,Modules,Module,Id,Items,Id,Mark,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsidmark-read-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodulesmodule-iditemsidmark-read-post-openapi.md
- name: Instructure Canvas Courses API Get module item sequence
  x-api-slug: instructure-canvas-courses-api
  description: Get module item sequence.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/module_item_sequence
  tags: Courses,Course,Id,Module,Item,Sequence
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodule-item-sequence-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idmodule-item-sequence-get-openapi.md
- name: Instructure Canvas Courses API Get all outcome groups for context
  x-api-slug: instructure-canvas-courses-api
  description: Get all outcome groups for context.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups
  tags: Courses,Course,Id,Outcome,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groups-get-openapi.md
- name: Instructure Canvas Courses API Delete an outcome group
  x-api-slug: instructure-canvas-courses-api
  description: Delete an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id
  tags: Courses,Course,Id,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsid-delete-openapi.md
- name: Instructure Canvas Courses API Show an outcome group
  x-api-slug: instructure-canvas-courses-api
  description: Show an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id
  tags: Courses,Course,Id,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsid-get-openapi.md
- name: Instructure Canvas Courses API Update an outcome group
  x-api-slug: instructure-canvas-courses-api
  description: Update an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id
  tags: Courses,Course,Id,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsid-put-openapi.md
- name: Instructure Canvas Courses API Import an outcome group
  x-api-slug: instructure-canvas-courses-api
  description: Import an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/import
  tags: Courses,Course,Id,Outcome,Groups,Id,Import
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidimport-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidimport-post-openapi.md
- name: Instructure Canvas Courses API List linked outcomes
  x-api-slug: instructure-canvas-courses-api
  description: List linked outcomes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/outcomes
  tags: Courses,Course,Id,Outcome,Groups,Id,Outcomes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomes-get-openapi.md
- name: Instructure Canvas Courses API Create/link an outcome
  x-api-slug: instructure-canvas-courses-api
  description: Create/link an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/outcomes
  tags: Courses,Course,Id,Outcome,Groups,Id,Outcomes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomes-post-openapi.md
- name: Instructure Canvas Courses API Unlink an outcome
  x-api-slug: instructure-canvas-courses-api
  description: Unlink an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/outcomes/{outcome_id}
  tags: Courses,Course,Id,Outcome,Groups,Id,Outcomes,Outcome,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomesoutcome-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomesoutcome-id-delete-openapi.md
- name: Instructure Canvas Courses API Create/link an outcome
  x-api-slug: instructure-canvas-courses-api
  description: Create/link an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/outcomes/{outcome_id}
  tags: Courses,Course,Id,Outcome,Groups,Id,Outcomes,Outcome,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomesoutcome-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidoutcomesoutcome-id-put-openapi.md
- name: Instructure Canvas Courses API List subgroups
  x-api-slug: instructure-canvas-courses-api
  description: List subgroups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/subgroups
  tags: Courses,Course,Id,Outcome,Groups,Id,Subgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidsubgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidsubgroups-get-openapi.md
- name: Instructure Canvas Courses API Create a subgroup
  x-api-slug: instructure-canvas-courses-api
  description: Create a subgroup.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_groups/id/subgroups
  tags: Courses,Course,Id,Outcome,Groups,Id,Subgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidsubgroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-groupsidsubgroups-post-openapi.md
- name: Instructure Canvas Courses API Get all outcome links for context
  x-api-slug: instructure-canvas-courses-api
  description: Get all outcome links for context.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_group_links
  tags: Courses,Course,Id,Outcome,Group,Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-group-links-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-group-links-get-openapi.md
- name: Instructure Canvas Courses API Get outcome results
  x-api-slug: instructure-canvas-courses-api
  description: Get outcome results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_results
  tags: Courses,Course,Id,Outcome,Results
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-results-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-results-get-openapi.md
- name: Instructure Canvas Courses API Get outcome result rollups
  x-api-slug: instructure-canvas-courses-api
  description: Get outcome result rollups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/outcome_rollups
  tags: Courses,Course,Id,Outcome,Rollups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-rollups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idoutcome-rollups-get-openapi.md
- name: Instructure Canvas Courses API List pages
  x-api-slug: instructure-canvas-courses-api
  description: List pages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/pages
  tags: Courses,Course,Id,Pages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpages-get-openapi.md
- name: Instructure Canvas Courses API Create page
  x-api-slug: instructure-canvas-courses-api
  description: Create page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/pages
  tags: Courses,Course,Id,Pages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpages-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpages-post-openapi.md
- name: Instructure Canvas Courses API Delete page
  x-api-slug: instructure-canvas-courses-api
  description: Delete page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/pages/url
  tags: Courses,Course,Id,Pages,Url
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurl-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurl-delete-openapi.md
- name: Instructure Canvas Courses API Show page
  x-api-slug: instructure-canvas-courses-api
  description: Show page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/pages/url
  tags: Courses,Course,Id,Pages,Url
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurl-get-openapi.md
- name: Instructure Canvas Courses API Update/create page
  x-api-slug: instructure-canvas-courses-api
  description: Update/create page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/pages/url
  tags: Courses,Course,Id,Pages,Url
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurl-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurl-put-openapi.md
- name: Instructure Canvas Courses API List revisions
  x-api-slug: instructure-canvas-courses-api
  description: List revisions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/pages/url/revisions
  tags: Courses,Course,Id,Pages,Url,Revisions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurlrevisions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurlrevisions-get-openapi.md
- name: Instructure Canvas Courses API Show revision
  x-api-slug: instructure-canvas-courses-api
  description: Show revision.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/pages/url/revisions/latest
  tags: Courses,Course,Id,Pages,Url,Revisions,Latest
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurlrevisionslatest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurlrevisionslatest-get-openapi.md
- name: Instructure Canvas Courses API Show revision
  x-api-slug: instructure-canvas-courses-api
  description: Show revision.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/pages/url/revisions/{revision_id}
  tags: Courses,Course,Id,Pages,Url,Revisions,Revision,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurlrevisionsrevision-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurlrevisionsrevision-id-get-openapi.md
- name: Instructure Canvas Courses API Revert to revision
  x-api-slug: instructure-canvas-courses-api
  description: Revert to revision.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/pages/url/revisions/{revision_id}
  tags: Courses,Course,Id,Pages,Url,Revisions,Revision,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurlrevisionsrevision-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpagesurlrevisionsrevision-id-post-openapi.md
- name: Instructure Canvas Courses API Preview processed html
  x-api-slug: instructure-canvas-courses-api
  description: Preview processed html.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/preview_html
  tags: Courses,Course,Id,Preview,Html
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpreview-html-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idpreview-html-post-openapi.md
- name: Instructure Canvas Courses API List quizzes in a course
  x-api-slug: instructure-canvas-courses-api
  description: List quizzes in a course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes
  tags: Courses,Course,Id,Quizzes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzes-get-openapi.md
- name: Instructure Canvas Courses API Create a quiz
  x-api-slug: instructure-canvas-courses-api
  description: Create a quiz.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes
  tags: Courses,Course,Id,Quizzes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzes-post-openapi.md
- name: Instructure Canvas Courses API Retrieve assignment-overridden dates for quizzes
  x-api-slug: instructure-canvas-courses-api
  description: Retrieve assignment-overridden dates for quizzes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/assignment_overrides
  tags: Courses,Course,Id,Quizzes,Assignment,Overrides
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesassignment-overrides-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesassignment-overrides-get-openapi.md
- name: Instructure Canvas Courses API Delete a quiz
  x-api-slug: instructure-canvas-courses-api
  description: Delete a quiz.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/id
  tags: Courses,Course,Id,Quizzes,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single quiz
  x-api-slug: instructure-canvas-courses-api
  description: Get a single quiz.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/id
  tags: Courses,Course,Id,Quizzes,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesid-get-openapi.md
- name: Instructure Canvas Courses API Edit a quiz
  x-api-slug: instructure-canvas-courses-api
  description: Edit a quiz.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/id
  tags: Courses,Course,Id,Quizzes,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesid-put-openapi.md
- name: Instructure Canvas Courses API Reorder quiz items
  x-api-slug: instructure-canvas-courses-api
  description: Reorder quiz items.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/id/reorder
  tags: Courses,Course,Id,Quizzes,Id,Reorder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesidreorder-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesidreorder-post-openapi.md
- name: Instructure Canvas Courses API Send a message to unsubmitted or submitted
    users for the quiz
  x-api-slug: instructure-canvas-courses-api
  description: Send a message to unsubmitted or submitted users for the quiz.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/id/submission_users/message
  tags: Courses,Course,Id,Quizzes,Id,Submission,Users,Message
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesidsubmission-usersmessage-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesidsubmission-usersmessage-post-openapi.md
- name: Instructure Canvas Courses API Validate quiz access code
  x-api-slug: instructure-canvas-courses-api
  description: Validate quiz access code.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/id/validate_access_code
  tags: Courses,Course,Id,Quizzes,Id,Validate,Access,Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesidvalidate-access-code-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesidvalidate-access-code-post-openapi.md
- name: Instructure Canvas Courses API Set extensions for student quiz submissions
  x-api-slug: instructure-canvas-courses-api
  description: Set extensions for student quiz submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/extensions
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Extensions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idextensions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idextensions-post-openapi.md
- name: Instructure Canvas Courses API Create a question group
  x-api-slug: instructure-canvas-courses-api
  description: Create a question group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroups-post-openapi.md
- name: Instructure Canvas Courses API Delete a question group
  x-api-slug: instructure-canvas-courses-api
  description: Delete a question group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single quiz group
  x-api-slug: instructure-canvas-courses-api
  description: Get a single quiz group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-get-openapi.md
- name: Instructure Canvas Courses API Update a question group
  x-api-slug: instructure-canvas-courses-api
  description: Update a question group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsid-put-openapi.md
- name: Instructure Canvas Courses API Reorder question groups
  x-api-slug: instructure-canvas-courses-api
  description: Reorder question groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/groups/{id}/reorder
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Groups,Id,Reorder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsidreorder-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idgroupsidreorder-post-openapi.md
- name: Instructure Canvas Courses API Get available quiz IP filters.
  x-api-slug: instructure-canvas-courses-api
  description: Get available quiz ip filters..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/ip_filters
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Ip,Filters
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idip-filters-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idip-filters-get-openapi.md
- name: Instructure Canvas Courses API List questions in a quiz or a submission
  x-api-slug: instructure-canvas-courses-api
  description: List questions in a quiz or a submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/questions
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestions-get-openapi.md
- name: Instructure Canvas Courses API Create a single quiz question
  x-api-slug: instructure-canvas-courses-api
  description: Create a single quiz question.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/questions
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestions-post-openapi.md
- name: Instructure Canvas Courses API Delete a quiz question
  x-api-slug: instructure-canvas-courses-api
  description: Delete a quiz question.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/questions/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Questions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestionsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestionsid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single quiz question
  x-api-slug: instructure-canvas-courses-api
  description: Get a single quiz question.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/questions/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Questions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestionsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestionsid-get-openapi.md
- name: Instructure Canvas Courses API Update an existing quiz question
  x-api-slug: instructure-canvas-courses-api
  description: Update an existing quiz question.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/questions/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Questions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestionsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idquestionsid-put-openapi.md
- name: Instructure Canvas Courses API Retrieve all quiz reports
  x-api-slug: instructure-canvas-courses-api
  description: Retrieve all quiz reports.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/reports
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idreports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idreports-get-openapi.md
- name: Instructure Canvas Courses API Create a quiz report
  x-api-slug: instructure-canvas-courses-api
  description: Create a quiz report.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/reports
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idreports-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idreports-post-openapi.md
- name: Instructure Canvas Courses API Abort the generation of a report, or remove
    a previously generated one
  x-api-slug: instructure-canvas-courses-api
  description: Abort the generation of a report, or remove a previously generated
    one.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/reports/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Reports,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idreportsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idreportsid-delete-openapi.md
- name: Instructure Canvas Courses API Get a quiz report
  x-api-slug: instructure-canvas-courses-api
  description: Get a quiz report.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/reports/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Reports,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idreportsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idreportsid-get-openapi.md
- name: Instructure Canvas Courses API Fetching the latest quiz statistics
  x-api-slug: instructure-canvas-courses-api
  description: Fetching the latest quiz statistics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/statistics
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Statistics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idstatistics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idstatistics-get-openapi.md
- name: Instructure Canvas Courses API Get all quiz submissions.
  x-api-slug: instructure-canvas-courses-api
  description: Get all quiz submissions..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissions-get-openapi.md
- name: Instructure Canvas Courses API Create the quiz submission (start a quiz-taking
    session)
  x-api-slug: instructure-canvas-courses-api
  description: Create the quiz submission (start a quiz-taking session).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissions-post-openapi.md
- name: Instructure Canvas Courses API Upload a file
  x-api-slug: instructure-canvas-courses-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions/self/files
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions,Self,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsselffiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsselffiles-post-openapi.md
- name: Instructure Canvas Courses API Get a single quiz submission.
  x-api-slug: instructure-canvas-courses-api
  description: Get a single quiz submission..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsid-get-openapi.md
- name: Instructure Canvas Courses API Update student question scores and comments.
  x-api-slug: instructure-canvas-courses-api
  description: Update student question scores and comments..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions/{id}
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsid-put-openapi.md
- name: Instructure Canvas Courses API Complete the quiz submission (turn it in).
  x-api-slug: instructure-canvas-courses-api
  description: Complete the quiz submission (turn it in)..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions/{id}/complete
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions,Id,Complete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidcomplete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidcomplete-post-openapi.md
- name: Instructure Canvas Courses API Retrieve captured events
  x-api-slug: instructure-canvas-courses-api
  description: Retrieve captured events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions/{id}/events
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions,Id,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidevents-get-openapi.md
- name: Instructure Canvas Courses API Submit captured events
  x-api-slug: instructure-canvas-courses-api
  description: Submit captured events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions/{id}/events
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions,Id,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidevents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidevents-post-openapi.md
- name: Instructure Canvas Courses API Get current quiz submission times.
  x-api-slug: instructure-canvas-courses-api
  description: Get current quiz submission times..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions/{id}/time
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions,Id,Time
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidtime-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidtime-get-openapi.md
- name: Instructure Canvas Courses API Set extensions for student quiz submissions
  x-api-slug: instructure-canvas-courses-api
  description: Set extensions for student quiz submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quiz_extensions
  tags: Courses,Course,Id,Quiz,Extensions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquiz-extensions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idquiz-extensions-post-openapi.md
- name: Instructure Canvas Courses API List recently logged in students
  x-api-slug: instructure-canvas-courses-api
  description: List recently logged in students.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/recent_students
  tags: Courses,Course,Id,Recent,Students
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idrecent-students-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idrecent-students-get-openapi.md
- name: Instructure Canvas Courses API Reset a course
  x-api-slug: instructure-canvas-courses-api
  description: Reset a course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/reset_content
  tags: Courses,Course,Id,Reset,Content
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idreset-content-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idreset-content-post-openapi.md
- name: Instructure Canvas Courses API Redirect to root outcome group for context
  x-api-slug: instructure-canvas-courses-api
  description: Redirect to root outcome group for context.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/root_outcome_group
  tags: Courses,Course,Id,Root,Outcome,Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idroot-outcome-group-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idroot-outcome-group-get-openapi.md
- name: Instructure Canvas Courses API List users in course
  x-api-slug: instructure-canvas-courses-api
  description: List users in course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/search_users
  tags: Courses,Course,Id,Search,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsearch-users-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsearch-users-get-openapi.md
- name: Instructure Canvas Courses API List course sections
  x-api-slug: instructure-canvas-courses-api
  description: List course sections.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/sections
  tags: Courses,Course,Id,Sections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsections-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsections-get-openapi.md
- name: Instructure Canvas Courses API Create course section
  x-api-slug: instructure-canvas-courses-api
  description: Create course section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/sections
  tags: Courses,Course,Id,Sections
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsections-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsections-post-openapi.md
- name: Instructure Canvas Courses API Get section information
  x-api-slug: instructure-canvas-courses-api
  description: Get section information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/sections/id
  tags: Courses,Course,Id,Sections,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsectionsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsectionsid-get-openapi.md
- name: Instructure Canvas Courses API Get course settings
  x-api-slug: instructure-canvas-courses-api
  description: Get course settings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/settings
  tags: Courses,Course,Id,Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsettings-get-openapi.md
- name: Instructure Canvas Courses API Update course settings
  x-api-slug: instructure-canvas-courses-api
  description: Update course settings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/settings
  tags: Courses,Course,Id,Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsettings-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsettings-put-openapi.md
- name: Instructure Canvas Courses API List students
  x-api-slug: instructure-canvas-courses-api
  description: List students.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/students
  tags: Courses,Course,Id,Students
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idstudents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idstudents-get-openapi.md
- name: Instructure Canvas Courses API List submissions for multiple assignments
  x-api-slug: instructure-canvas-courses-api
  description: List submissions for multiple assignments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/students/submissions
  tags: Courses,Course,Id,Students,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idstudentssubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idstudentssubmissions-get-openapi.md
- name: Instructure Canvas Courses API Grade or comment on multiple submissions
  x-api-slug: instructure-canvas-courses-api
  description: Grade or comment on multiple submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/submissions/update_grades
  tags: Courses,Course,Id,Submissions,Update,Grades
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsubmissionsupdate-grades-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idsubmissionsupdate-grades-post-openapi.md
- name: Instructure Canvas Courses API List available tabs for a course or group
  x-api-slug: instructure-canvas-courses-api
  description: List available tabs for a course or group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/tabs
  tags: Courses,Course,Id,Tabs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idtabs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idtabs-get-openapi.md
- name: Instructure Canvas Courses API Update a tab for a course
  x-api-slug: instructure-canvas-courses-api
  description: Update a tab for a course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/tabs/tab_id
  tags: Courses,Course,Id,Tabs,Tab,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idtabstab-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idtabstab-id-put-openapi.md
- name: Instructure Canvas Courses API Course TODO items
  x-api-slug: instructure-canvas-courses-api
  description: Course todo items.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/todo
  tags: Courses,Course,Id,Todo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idtodo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idtodo-get-openapi.md
- name: Instructure Canvas Courses API Remove usage rights
  x-api-slug: instructure-canvas-courses-api
  description: Remove usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/usage_rights
  tags: Courses,Course,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idusage-rights-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idusage-rights-delete-openapi.md
- name: Instructure Canvas Courses API Set usage rights
  x-api-slug: instructure-canvas-courses-api
  description: Set usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/usage_rights
  tags: Courses,Course,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idusage-rights-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idusage-rights-put-openapi.md
- name: Instructure Canvas Courses API List users in course
  x-api-slug: instructure-canvas-courses-api
  description: List users in course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/users
  tags: Courses,Course,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idusers-get-openapi.md
- name: Instructure Canvas Courses API Get single user
  x-api-slug: instructure-canvas-courses-api
  description: Get single user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/users/id
  tags: Courses,Course,Id,Users,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idusersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursescourse-idusersid-get-openapi.md
- name: Instructure Canvas Courses API Conclude a course
  x-api-slug: instructure-canvas-courses-api
  description: Conclude a course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{id}
  tags: Courses,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursesid-delete-openapi.md
- name: Instructure Canvas Courses API Get a single course
  x-api-slug: instructure-canvas-courses-api
  description: Get a single course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{id}
  tags: Courses,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursesid-get-openapi.md
- name: Instructure Canvas Courses API Update a course
  x-api-slug: instructure-canvas-courses-api
  description: Update a course.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{id}
  tags: Courses,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/coursesid-put-openapi.md
- name: Instructure Canvas Courses API
  x-api-slug: instructure-canvas-courses-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Global API Delete an outcome group
  x-api-slug: instructure-canvas-global-api
  description: Delete an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}
  tags: Global,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsid-delete-openapi.md
- name: Instructure Canvas Global API Show an outcome group
  x-api-slug: instructure-canvas-global-api
  description: Show an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}
  tags: Global,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsid-get-openapi.md
- name: Instructure Canvas Global API Update an outcome group
  x-api-slug: instructure-canvas-global-api
  description: Update an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}
  tags: Global,Outcome,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsid-put-openapi.md
- name: Instructure Canvas Global API Import an outcome group
  x-api-slug: instructure-canvas-global-api
  description: Import an outcome group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/import
  tags: Global,Outcome,Groups,Id,Import
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidimport-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidimport-post-openapi.md
- name: Instructure Canvas Global API List linked outcomes
  x-api-slug: instructure-canvas-global-api
  description: List linked outcomes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/outcomes
  tags: Global,Outcome,Groups,Id,Outcomes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidoutcomes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidoutcomes-get-openapi.md
- name: Instructure Canvas Global API Create/link an outcome
  x-api-slug: instructure-canvas-global-api
  description: Create/link an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/outcomes
  tags: Global,Outcome,Groups,Id,Outcomes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidoutcomes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidoutcomes-post-openapi.md
- name: Instructure Canvas Global API Unlink an outcome
  x-api-slug: instructure-canvas-global-api
  description: Unlink an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/outcomes/outcome_id
  tags: Global,Outcome,Groups,Id,Outcomes,Outcome,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidoutcomesoutcome-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidoutcomesoutcome-id-delete-openapi.md
- name: Instructure Canvas Global API Create/link an outcome
  x-api-slug: instructure-canvas-global-api
  description: Create/link an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/outcomes/outcome_id
  tags: Global,Outcome,Groups,Id,Outcomes,Outcome,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidoutcomesoutcome-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidoutcomesoutcome-id-put-openapi.md
- name: Instructure Canvas Global API List subgroups
  x-api-slug: instructure-canvas-global-api
  description: List subgroups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/subgroups
  tags: Global,Outcome,Groups,Id,Subgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidsubgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidsubgroups-get-openapi.md
- name: Instructure Canvas Global API Create a subgroup
  x-api-slug: instructure-canvas-global-api
  description: Create a subgroup.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/outcome_groups/{id}/subgroups
  tags: Global,Outcome,Groups,Id,Subgroups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidsubgroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globaloutcome-groupsidsubgroups-post-openapi.md
- name: Instructure Canvas Global API Redirect to root outcome group for context
  x-api-slug: instructure-canvas-global-api
  description: Redirect to root outcome group for context.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//global/root_outcome_group
  tags: Global,Root,Outcome,Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globalroot-outcome-group-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/globalroot-outcome-group-get-openapi.md
- name: Instructure Canvas Global API
  x-api-slug: instructure-canvas-global-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Groups API Create a group
  x-api-slug: instructure-canvas-groups-api
  description: Create a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups
  tags: Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groups-post-openapi.md
- name: Instructure Canvas Groups API Delete a group
  x-api-slug: instructure-canvas-groups-api
  description: Delete a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}
  tags: Groups,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single group
  x-api-slug: instructure-canvas-groups-api
  description: Get a single group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}
  tags: Groups,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-id-get-openapi.md
- name: Instructure Canvas Groups API Edit a group
  x-api-slug: instructure-canvas-groups-api
  description: Edit a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}
  tags: Groups,Group,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-id-put-openapi.md
- name: Instructure Canvas Groups API Group activity stream
  x-api-slug: instructure-canvas-groups-api
  description: Group activity stream.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/activity_stream
  tags: Groups,Group,Id,Activity,Stream
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idactivity-stream-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idactivity-stream-get-openapi.md
- name: Instructure Canvas Groups API Group activity stream summary
  x-api-slug: instructure-canvas-groups-api
  description: Group activity stream summary.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/activity_stream/summary
  tags: Groups,Group,Id,Activity,Stream,Summary
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idactivity-streamsummary-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idactivity-streamsummary-get-openapi.md
- name: Instructure Canvas Groups API Redirect to the assignment override for a group
  x-api-slug: instructure-canvas-groups-api
  description: Redirect to the assignment override for a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/assignments/assignment_id/override
  tags: Groups,Group,Id,Assignments,Assignment,Id,Override
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idassignmentsassignment-idoverride-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idassignmentsassignment-idoverride-get-openapi.md
- name: Instructure Canvas Groups API List conferences
  x-api-slug: instructure-canvas-groups-api
  description: List conferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/conferences
  tags: Groups,Group,Id,Conferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idconferences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idconferences-get-openapi.md
- name: Instructure Canvas Groups API List content exports
  x-api-slug: instructure-canvas-groups-api
  description: List content exports.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_exports
  tags: Groups,Group,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-exports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-exports-get-openapi.md
- name: Instructure Canvas Groups API Export content
  x-api-slug: instructure-canvas-groups-api
  description: Export content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_exports
  tags: Groups,Group,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-exports-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-exports-post-openapi.md
- name: Instructure Canvas Groups API Show content export
  x-api-slug: instructure-canvas-groups-api
  description: Show content export.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_exports/id
  tags: Groups,Group,Id,Content,Exports,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-exportsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-exportsid-get-openapi.md
- name: Instructure Canvas Groups API List licenses
  x-api-slug: instructure-canvas-groups-api
  description: List licenses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_licenses
  tags: Groups,Group,Id,Content,Licenses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-licenses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-licenses-get-openapi.md
- name: Instructure Canvas Groups API List content migrations
  x-api-slug: instructure-canvas-groups-api
  description: List content migrations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations
  tags: Groups,Group,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrations-get-openapi.md
- name: Instructure Canvas Groups API Create a content migration
  x-api-slug: instructure-canvas-groups-api
  description: Create a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations
  tags: Groups,Group,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrations-post-openapi.md
- name: Instructure Canvas Groups API List migration issues
  x-api-slug: instructure-canvas-groups-api
  description: List migration issues.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/content_migration_id/migration_issues
  tags: Groups,Group,Id,Content,Migrations,Content,Migration,Id,Migration,Issues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issues-get-openapi.md
- name: Instructure Canvas Groups API Get a migration issue
  x-api-slug: instructure-canvas-groups-api
  description: Get a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Groups,Group,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-get-openapi.md
- name: Instructure Canvas Groups API Update a migration issue
  x-api-slug: instructure-canvas-groups-api
  description: Update a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Groups,Group,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationscontent-migration-idmigration-issuesid-put-openapi.md
- name: Instructure Canvas Groups API Get a content migration
  x-api-slug: instructure-canvas-groups-api
  description: Get a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/id
  tags: Groups,Group,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationsid-get-openapi.md
- name: Instructure Canvas Groups API Update a content migration
  x-api-slug: instructure-canvas-groups-api
  description: Update a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/id
  tags: Groups,Group,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationsid-put-openapi.md
- name: Instructure Canvas Groups API List Migration Systems
  x-api-slug: instructure-canvas-groups-api
  description: List migration systems.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/content_migrations/migrators
  tags: Groups,Group,Id,Content,Migrations,Migrators
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationsmigrators-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idcontent-migrationsmigrators-get-openapi.md
- name: Instructure Canvas Groups API List discussion topics
  x-api-slug: instructure-canvas-groups-api
  description: List discussion topics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics
  tags: Groups,Group,Id,Discussion,Topics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topics-get-openapi.md
- name: Instructure Canvas Groups API Create a new discussion topic
  x-api-slug: instructure-canvas-groups-api
  description: Create a new discussion topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics
  tags: Groups,Group,Id,Discussion,Topics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topics-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topics-post-openapi.md
- name: Instructure Canvas Groups API Reorder pinned topics
  x-api-slug: instructure-canvas-groups-api
  description: Reorder pinned topics.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/reorder
  tags: Groups,Group,Id,Discussion,Topics,Reorder
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicsreorder-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicsreorder-post-openapi.md
- name: Instructure Canvas Groups API Delete a topic
  x-api-slug: instructure-canvas-groups-api
  description: Delete a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single topic
  x-api-slug: instructure-canvas-groups-api
  description: Get a single topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-get-openapi.md
- name: Instructure Canvas Groups API Update a topic
  x-api-slug: instructure-canvas-groups-api
  description: Update a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-id-put-openapi.md
- name: Instructure Canvas Groups API List topic entries
  x-api-slug: instructure-canvas-groups-api
  description: List topic entries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identries-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identries-get-openapi.md
- name: Instructure Canvas Groups API Post an entry
  x-api-slug: instructure-canvas-groups-api
  description: Post an entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identries-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identries-post-openapi.md
- name: Instructure Canvas Groups API Rate entry
  x-api-slug: instructure-canvas-groups-api
  description: Rate entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/rating
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Rating
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idrating-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idrating-post-openapi.md
- name: Instructure Canvas Groups API Mark entry as unread
  x-api-slug: instructure-canvas-groups-api
  description: Mark entry as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/read
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idread-delete-openapi.md
- name: Instructure Canvas Groups API Mark entry as read
  x-api-slug: instructure-canvas-groups-api
  description: Mark entry as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/read
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idread-put-openapi.md
- name: Instructure Canvas Groups API List entry replies
  x-api-slug: instructure-canvas-groups-api
  description: List entry replies.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/replies
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Replies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-get-openapi.md
- name: Instructure Canvas Groups API Post a reply
  x-api-slug: instructure-canvas-groups-api
  description: Post a reply.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/replies
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Entry,Id,Replies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesentry-idreplies-post-openapi.md
- name: Instructure Canvas Groups API Delete an entry
  x-api-slug: instructure-canvas-groups-api
  description: Delete an entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{id}
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesid-delete-openapi.md
- name: Instructure Canvas Groups API Update an entry
  x-api-slug: instructure-canvas-groups-api
  description: Update an entry.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entries/{id}
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entries,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identriesid-put-openapi.md
- name: Instructure Canvas Groups API List entries
  x-api-slug: instructure-canvas-groups-api
  description: List entries.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/entry_list
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Entry,List
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identry-list-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-identry-list-get-openapi.md
- name: Instructure Canvas Groups API Mark topic as unread
  x-api-slug: instructure-canvas-groups-api
  description: Mark topic as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/read
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-delete-openapi.md
- name: Instructure Canvas Groups API Mark topic as read
  x-api-slug: instructure-canvas-groups-api
  description: Mark topic as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/read
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-put-openapi.md
- name: Instructure Canvas Groups API Mark all entries as unread
  x-api-slug: instructure-canvas-groups-api
  description: Mark all entries as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/read_all
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-all-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-all-delete-openapi.md
- name: Instructure Canvas Groups API Mark all entries as read
  x-api-slug: instructure-canvas-groups-api
  description: Mark all entries as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/read_all
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-all-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idread-all-put-openapi.md
- name: Instructure Canvas Groups API Unsubscribe from a topic
  x-api-slug: instructure-canvas-groups-api
  description: Unsubscribe from a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/subscribed
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Subscribed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idsubscribed-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idsubscribed-delete-openapi.md
- name: Instructure Canvas Groups API Subscribe to a topic
  x-api-slug: instructure-canvas-groups-api
  description: Subscribe to a topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/subscribed
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,Subscribed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idsubscribed-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idsubscribed-put-openapi.md
- name: Instructure Canvas Groups API Get the full topic
  x-api-slug: instructure-canvas-groups-api
  description: Get the full topic.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/discussion_topics/topic_id/view
  tags: Groups,Group,Id,Discussion,Topics,Topic,Id,View
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idview-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-iddiscussion-topicstopic-idview-get-openapi.md
- name: Instructure Canvas Groups API List external feeds
  x-api-slug: instructure-canvas-groups-api
  description: List external feeds.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/external_feeds
  tags: Groups,Group,Id,External,Feeds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idexternal-feeds-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idexternal-feeds-get-openapi.md
- name: Instructure Canvas Groups API Create an external feed
  x-api-slug: instructure-canvas-groups-api
  description: Create an external feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/external_feeds
  tags: Groups,Group,Id,External,Feeds
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idexternal-feeds-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idexternal-feeds-post-openapi.md
- name: Instructure Canvas Groups API Delete an external feed
  x-api-slug: instructure-canvas-groups-api
  description: Delete an external feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/external_feeds/external_feed_id
  tags: Groups,Group,Id,External,Feeds,External,Feed,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idexternal-feedsexternal-feed-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idexternal-feedsexternal-feed-id-delete-openapi.md
- name: Instructure Canvas Groups API List files
  x-api-slug: instructure-canvas-groups-api
  description: List files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/files
  tags: Groups,Group,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfiles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfiles-get-openapi.md
- name: Instructure Canvas Groups API Upload a file
  x-api-slug: instructure-canvas-groups-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/files
  tags: Groups,Group,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfiles-post-openapi.md
- name: Instructure Canvas Groups API Get file
  x-api-slug: instructure-canvas-groups-api
  description: Get file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/files/id
  tags: Groups,Group,Id,Files,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfilesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfilesid-get-openapi.md
- name: Instructure Canvas Groups API Get quota information
  x-api-slug: instructure-canvas-groups-api
  description: Get quota information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/files/quota
  tags: Groups,Group,Id,Files,Quota
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfilesquota-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfilesquota-get-openapi.md
- name: Instructure Canvas Groups API List all folders
  x-api-slug: instructure-canvas-groups-api
  description: List all folders.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders
  tags: Groups,Group,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfolders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfolders-get-openapi.md
- name: Instructure Canvas Groups API Create folder
  x-api-slug: instructure-canvas-groups-api
  description: Create folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders
  tags: Groups,Group,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfolders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfolders-post-openapi.md
- name: Instructure Canvas Groups API Resolve path
  x-api-slug: instructure-canvas-groups-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders/by_path
  tags: Groups,Group,Id,Folders,By,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfoldersby-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfoldersby-path-get-openapi.md
- name: Instructure Canvas Groups API Resolve path
  x-api-slug: instructure-canvas-groups-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders/by_path/*full_path
  tags: Groups,Group,Id,Folders,By,Path,*full,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfoldersby-pathfull-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfoldersby-pathfull-path-get-openapi.md
- name: Instructure Canvas Groups API Get folder
  x-api-slug: instructure-canvas-groups-api
  description: Get folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/folders/id
  tags: Groups,Group,Id,Folders,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfoldersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfoldersid-get-openapi.md
- name: Instructure Canvas Groups API Show front page
  x-api-slug: instructure-canvas-groups-api
  description: Show front page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/front_page
  tags: Groups,Group,Id,Front,Page
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfront-page-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfront-page-get-openapi.md
- name: Instructure Canvas Groups API Update/create front page
  x-api-slug: instructure-canvas-groups-api
  description: Update/create front page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/front_page
  tags: Groups,Group,Id,Front,Page
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfront-page-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idfront-page-put-openapi.md
- name: Instructure Canvas Groups API Invite others to a group
  x-api-slug: instructure-canvas-groups-api
  description: Invite others to a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/invite
  tags: Groups,Group,Id,Invite
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idinvite-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idinvite-post-openapi.md
- name: Instructure Canvas Groups API List group memberships
  x-api-slug: instructure-canvas-groups-api
  description: List group memberships.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships
  tags: Groups,Group,Id,Memberships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmemberships-get-openapi.md
- name: Instructure Canvas Groups API Create a membership
  x-api-slug: instructure-canvas-groups-api
  description: Create a membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships
  tags: Groups,Group,Id,Memberships
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmemberships-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmemberships-post-openapi.md
- name: Instructure Canvas Groups API Leave a group
  x-api-slug: instructure-canvas-groups-api
  description: Leave a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships/membership_id
  tags: Groups,Group,Id,Memberships,Membership,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single group membership
  x-api-slug: instructure-canvas-groups-api
  description: Get a single group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships/membership_id
  tags: Groups,Group,Id,Memberships,Membership,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-get-openapi.md
- name: Instructure Canvas Groups API Update a membership
  x-api-slug: instructure-canvas-groups-api
  description: Update a membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/memberships/membership_id
  tags: Groups,Group,Id,Memberships,Membership,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idmembershipsmembership-id-put-openapi.md
- name: Instructure Canvas Groups API List pages
  x-api-slug: instructure-canvas-groups-api
  description: List pages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages
  tags: Groups,Group,Id,Pages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpages-get-openapi.md
- name: Instructure Canvas Groups API Create page
  x-api-slug: instructure-canvas-groups-api
  description: Create page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages
  tags: Groups,Group,Id,Pages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpages-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpages-post-openapi.md
- name: Instructure Canvas Groups API Delete page
  x-api-slug: instructure-canvas-groups-api
  description: Delete page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url
  tags: Groups,Group,Id,Pages,Url
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurl-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurl-delete-openapi.md
- name: Instructure Canvas Groups API Show page
  x-api-slug: instructure-canvas-groups-api
  description: Show page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url
  tags: Groups,Group,Id,Pages,Url
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurl-get-openapi.md
- name: Instructure Canvas Groups API Update/create page
  x-api-slug: instructure-canvas-groups-api
  description: Update/create page.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url
  tags: Groups,Group,Id,Pages,Url
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurl-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurl-put-openapi.md
- name: Instructure Canvas Groups API List revisions
  x-api-slug: instructure-canvas-groups-api
  description: List revisions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url/revisions
  tags: Groups,Group,Id,Pages,Url,Revisions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurlrevisions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurlrevisions-get-openapi.md
- name: Instructure Canvas Groups API Show revision
  x-api-slug: instructure-canvas-groups-api
  description: Show revision.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url/revisions/latest
  tags: Groups,Group,Id,Pages,Url,Revisions,Latest
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurlrevisionslatest-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurlrevisionslatest-get-openapi.md
- name: Instructure Canvas Groups API Show revision
  x-api-slug: instructure-canvas-groups-api
  description: Show revision.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url/revisions/{revision_id}
  tags: Groups,Group,Id,Pages,Url,Revisions,Revision,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurlrevisionsrevision-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurlrevisionsrevision-id-get-openapi.md
- name: Instructure Canvas Groups API Revert to revision
  x-api-slug: instructure-canvas-groups-api
  description: Revert to revision.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/pages/url/revisions/{revision_id}
  tags: Groups,Group,Id,Pages,Url,Revisions,Revision,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurlrevisionsrevision-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpagesurlrevisionsrevision-id-post-openapi.md
- name: Instructure Canvas Groups API Preview processed html
  x-api-slug: instructure-canvas-groups-api
  description: Preview processed html.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/preview_html
  tags: Groups,Group,Id,Preview,Html
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpreview-html-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idpreview-html-post-openapi.md
- name: Instructure Canvas Groups API List available tabs for a course or group
  x-api-slug: instructure-canvas-groups-api
  description: List available tabs for a course or group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/tabs
  tags: Groups,Group,Id,Tabs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idtabs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idtabs-get-openapi.md
- name: Instructure Canvas Groups API Remove usage rights
  x-api-slug: instructure-canvas-groups-api
  description: Remove usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/usage_rights
  tags: Groups,Group,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusage-rights-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusage-rights-delete-openapi.md
- name: Instructure Canvas Groups API Set usage rights
  x-api-slug: instructure-canvas-groups-api
  description: Set usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/usage_rights
  tags: Groups,Group,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusage-rights-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusage-rights-put-openapi.md
- name: Instructure Canvas Groups API List groups users
  x-api-slug: instructure-canvas-groups-api
  description: List groups users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users
  tags: Groups,Group,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusers-get-openapi.md
- name: Instructure Canvas Groups API Leave a group
  x-api-slug: instructure-canvas-groups-api
  description: Leave a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users/user_id
  tags: Groups,Group,Id,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusersuser-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusersuser-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single group membership
  x-api-slug: instructure-canvas-groups-api
  description: Get a single group membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users/user_id
  tags: Groups,Group,Id,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusersuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusersuser-id-get-openapi.md
- name: Instructure Canvas Groups API Update a membership
  x-api-slug: instructure-canvas-groups-api
  description: Update a membership.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//groups/{group_id}/users/user_id
  tags: Groups,Group,Id,Users,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusersuser-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/groupsgroup-idusersuser-id-put-openapi.md
- name: Instructure Canvas Groups API Delete a Group Category
  x-api-slug: instructure-canvas-groups-api
  description: Delete a group category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}
  tags: Group,Categories,Group,Category,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-id-delete-openapi.md
- name: Instructure Canvas Groups API Get a single group category
  x-api-slug: instructure-canvas-groups-api
  description: Get a single group category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}
  tags: Group,Categories,Group,Category,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-id-get-openapi.md
- name: Instructure Canvas Groups API Update a Group Category
  x-api-slug: instructure-canvas-groups-api
  description: Update a group category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}
  tags: Group,Categories,Group,Category,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-id-put-openapi.md
- name: Instructure Canvas Groups API Assign unassigned members
  x-api-slug: instructure-canvas-groups-api
  description: Assign unassigned members.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}/assign_unassigned_members
  tags: Group,Categories,Group,Category,Id,Assign,Unassigned,Members
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-idassign-unassigned-members-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-idassign-unassigned-members-post-openapi.md
- name: Instructure Canvas Groups API List groups in group category
  x-api-slug: instructure-canvas-groups-api
  description: List groups in group category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}/groups
  tags: Group,Categories,Group,Category,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-idgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-idgroups-get-openapi.md
- name: Instructure Canvas Groups API Create a group
  x-api-slug: instructure-canvas-groups-api
  description: Create a group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}/groups
  tags: Group,Categories,Group,Category,Id,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-idgroups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-idgroups-post-openapi.md
- name: Instructure Canvas Groups API List users in group category
  x-api-slug: instructure-canvas-groups-api
  description: List users in group category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//group_categories/{group_category_id}/users
  tags: Group,Categories,Group,Category,Id,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-idusers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/group-categoriesgroup-category-idusers-get-openapi.md
- name: Instructure Canvas Groups API
  x-api-slug: instructure-canvas-groups-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Polls API List polls
  x-api-slug: instructure-canvas-polls-api
  description: List polls.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls
  tags: Polls
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/polls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/polls-get-openapi.md
- name: Instructure Canvas Polls API Create a single poll
  x-api-slug: instructure-canvas-polls-api
  description: Create a single poll.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls
  tags: Polls
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/polls-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/polls-post-openapi.md
- name: Instructure Canvas Polls API Delete a poll
  x-api-slug: instructure-canvas-polls-api
  description: Delete a poll.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{id}
  tags: Polls,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollsid-delete-openapi.md
- name: Instructure Canvas Polls API Get a single poll
  x-api-slug: instructure-canvas-polls-api
  description: Get a single poll.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{id}
  tags: Polls,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollsid-get-openapi.md
- name: Instructure Canvas Polls API Update a single poll
  x-api-slug: instructure-canvas-polls-api
  description: Update a single poll.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{id}
  tags: Polls,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollsid-put-openapi.md
- name: Instructure Canvas Polls API List poll choices in a poll
  x-api-slug: instructure-canvas-polls-api
  description: List poll choices in a poll.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_choices
  tags: Polls,Poll,Id,Poll,Choices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choices-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choices-get-openapi.md
- name: Instructure Canvas Polls API Create a single poll choice
  x-api-slug: instructure-canvas-polls-api
  description: Create a single poll choice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_choices
  tags: Polls,Poll,Id,Poll,Choices
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choices-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choices-post-openapi.md
- name: Instructure Canvas Polls API Delete a poll choice
  x-api-slug: instructure-canvas-polls-api
  description: Delete a poll choice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_choices/id
  tags: Polls,Poll,Id,Poll,Choices,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choicesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choicesid-delete-openapi.md
- name: Instructure Canvas Polls API Get a single poll choice
  x-api-slug: instructure-canvas-polls-api
  description: Get a single poll choice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_choices/id
  tags: Polls,Poll,Id,Poll,Choices,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choicesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choicesid-get-openapi.md
- name: Instructure Canvas Polls API Update a single poll choice
  x-api-slug: instructure-canvas-polls-api
  description: Update a single poll choice.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_choices/id
  tags: Polls,Poll,Id,Poll,Choices,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choicesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-choicesid-put-openapi.md
- name: Instructure Canvas Polls API List poll sessions for a poll
  x-api-slug: instructure-canvas-polls-api
  description: List poll sessions for a poll.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_sessions
  tags: Polls,Poll,Id,Poll,Sessions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessions-get-openapi.md
- name: Instructure Canvas Polls API Create a single poll session
  x-api-slug: instructure-canvas-polls-api
  description: Create a single poll session.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_sessions
  tags: Polls,Poll,Id,Poll,Sessions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessions-post-openapi.md
- name: Instructure Canvas Polls API Delete a poll session
  x-api-slug: instructure-canvas-polls-api
  description: Delete a poll session.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_sessions/id
  tags: Polls,Poll,Id,Poll,Sessions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsid-delete-openapi.md
- name: Instructure Canvas Polls API Get the results for a single poll session
  x-api-slug: instructure-canvas-polls-api
  description: Get the results for a single poll session.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_sessions/id
  tags: Polls,Poll,Id,Poll,Sessions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsid-get-openapi.md
- name: Instructure Canvas Polls API Update a single poll session
  x-api-slug: instructure-canvas-polls-api
  description: Update a single poll session.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_sessions/id
  tags: Polls,Poll,Id,Poll,Sessions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsid-put-openapi.md
- name: Instructure Canvas Polls API Close an opened poll session
  x-api-slug: instructure-canvas-polls-api
  description: Close an opened poll session.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_sessions/id/close
  tags: Polls,Poll,Id,Poll,Sessions,Id,Close
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsidclose-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsidclose-get-openapi.md
- name: Instructure Canvas Polls API Open a poll session
  x-api-slug: instructure-canvas-polls-api
  description: Open a poll session.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_sessions/id/open
  tags: Polls,Poll,Id,Poll,Sessions,Id,Open
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsidopen-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionsidopen-get-openapi.md
- name: Instructure Canvas Polls API Create a single poll submission
  x-api-slug: instructure-canvas-polls-api
  description: Create a single poll submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_sessions/poll_session_id/poll_submissions
  tags: Polls,Poll,Id,Poll,Sessions,Poll,Session,Id,Poll,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionspoll-session-idpoll-submissions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionspoll-session-idpoll-submissions-post-openapi.md
- name: Instructure Canvas Polls API Get a single poll submission
  x-api-slug: instructure-canvas-polls-api
  description: Get a single poll submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//polls/{poll_id}/poll_sessions/poll_session_id/poll_submissions/{id}
  tags: Polls,Poll,Id,Poll,Sessions,Poll,Session,Id,Poll,Submissions,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionspoll-session-idpoll-submissionsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/pollspoll-idpoll-sessionspoll-session-idpoll-submissionsid-get-openapi.md
- name: Instructure Canvas Polls API List closed poll sessions
  x-api-slug: instructure-canvas-polls-api
  description: List closed poll sessions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//poll_sessions/closed
  tags: Poll,Sessions,Closed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/poll-sessionsclosed-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/poll-sessionsclosed-get-openapi.md
- name: Instructure Canvas Polls API List opened poll sessions
  x-api-slug: instructure-canvas-polls-api
  description: List opened poll sessions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//poll_sessions/opened
  tags: Poll,Sessions,Opened
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/poll-sessionsopened-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/poll-sessionsopened-get-openapi.md
- name: Instructure Canvas Polls API
  x-api-slug: instructure-canvas-polls-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Quiz Submissions API Get all quiz submission questions.
  x-api-slug: instructure-canvas-quiz-submissions-api
  description: Get all quiz submission questions..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//quiz_submissions/{quiz_submission_id}/questions
  tags: Quiz,Submissions,Quiz,Submission,Id,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/quiz-submissionsquiz-submission-idquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/quiz-submissionsquiz-submission-idquestions-get-openapi.md
- name: Instructure Canvas Quiz Submissions API Answering questions
  x-api-slug: instructure-canvas-quiz-submissions-api
  description: Answering questions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//quiz_submissions/{quiz_submission_id}/questions
  tags: Quiz,Submissions,Quiz,Submission,Id,Questions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/quiz-submissionsquiz-submission-idquestions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/quiz-submissionsquiz-submission-idquestions-post-openapi.md
- name: Instructure Canvas Quiz Submissions API Flagging a question.
  x-api-slug: instructure-canvas-quiz-submissions-api
  description: Flagging a question..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//quiz_submissions/{quiz_submission_id}/questions/id/flag
  tags: Quiz,Submissions,Quiz,Submission,Id,Questions,Id,Flag
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/quiz-submissionsquiz-submission-idquestionsidflag-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/quiz-submissionsquiz-submission-idquestionsidflag-put-openapi.md
- name: Instructure Canvas Quiz Submissions API Unflagging a question.
  x-api-slug: instructure-canvas-quiz-submissions-api
  description: Unflagging a question..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//quiz_submissions/{quiz_submission_id}/questions/id/unflag
  tags: Quiz,Submissions,Quiz,Submission,Id,Questions,Id,Unflag
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/quiz-submissionsquiz-submission-idquestionsidunflag-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/quiz-submissionsquiz-submission-idquestionsidunflag-put-openapi.md
- name: Instructure Canvas Quiz Submissions API
  x-api-slug: instructure-canvas-quiz-submissions-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Sections API Redirect to the assignment override for a
    section
  x-api-slug: instructure-canvas-sections-api
  description: Redirect to the assignment override for a section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{course_section_id}/assignments/assignment_id/override
  tags: Sections,Course,Section,Id,Assignments,Assignment,Id,Override
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionscourse-section-idassignmentsassignment-idoverride-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionscourse-section-idassignmentsassignment-idoverride-get-openapi.md
- name: Instructure Canvas Sections API Delete a section
  x-api-slug: instructure-canvas-sections-api
  description: Delete a section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{id}
  tags: Sections,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsid-delete-openapi.md
- name: Instructure Canvas Sections API Get section information
  x-api-slug: instructure-canvas-sections-api
  description: Get section information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{id}
  tags: Sections,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsid-get-openapi.md
- name: Instructure Canvas Sections API Edit a section
  x-api-slug: instructure-canvas-sections-api
  description: Edit a section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{id}
  tags: Sections,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsid-put-openapi.md
- name: Instructure Canvas Sections API De-cross-list a Section
  x-api-slug: instructure-canvas-sections-api
  description: De-cross-list a section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{id}/crosslist
  tags: Sections,Id,Crosslist
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsidcrosslist-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsidcrosslist-delete-openapi.md
- name: Instructure Canvas Sections API Cross-list a Section
  x-api-slug: instructure-canvas-sections-api
  description: Cross-list a section.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{id}/crosslist/new_course_id
  tags: Sections,Id,Crosslist,New,Course,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsidcrosslistnew-course-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionsidcrosslistnew-course-id-post-openapi.md
- name: Instructure Canvas Sections API Get all Peer Reviews
  x-api-slug: instructure-canvas-sections-api
  description: Get all peer reviews.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/peer_reviews
  tags: Sections,Section,Id,Assignments,Assignment,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idpeer-reviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idpeer-reviews-get-openapi.md
- name: Instructure Canvas Sections API List assignment submissions
  x-api-slug: instructure-canvas-sections-api
  description: List assignment submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissions-get-openapi.md
- name: Instructure Canvas Sections API Submit an assignment
  x-api-slug: instructure-canvas-sections-api
  description: Submit an assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissions-post-openapi.md
- name: Instructure Canvas Sections API Grade or comment on multiple submissions
  x-api-slug: instructure-canvas-sections-api
  description: Grade or comment on multiple submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/update_grades
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,Update,Grades
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsupdate-grades-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsupdate-grades-post-openapi.md
- name: Instructure Canvas Sections API Create Peer Review
  x-api-slug: instructure-canvas-sections-api
  description: Create peer review.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-delete-openapi.md
- name: Instructure Canvas Sections API Get all Peer Reviews
  x-api-slug: instructure-canvas-sections-api
  description: Get all peer reviews.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-get-openapi.md
- name: Instructure Canvas Sections API Create Peer Review
  x-api-slug: instructure-canvas-sections-api
  description: Create peer review.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{submission_id}/peer_reviews
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,Submission,Id,Peer,Reviews
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionssubmission-idpeer-reviews-post-openapi.md
- name: Instructure Canvas Sections API Get a single submission
  x-api-slug: instructure-canvas-sections-api
  description: Get a single submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-id-get-openapi.md
- name: Instructure Canvas Sections API Grade or comment on a submission
  x-api-slug: instructure-canvas-sections-api
  description: Grade or comment on a submission.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-id-put-openapi.md
- name: Instructure Canvas Sections API Upload a file
  x-api-slug: instructure-canvas-sections-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}/files
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idfiles-post-openapi.md
- name: Instructure Canvas Sections API Mark submission as unread
  x-api-slug: instructure-canvas-sections-api
  description: Mark submission as unread.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}/read
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idread-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idread-delete-openapi.md
- name: Instructure Canvas Sections API Mark submission as read
  x-api-slug: instructure-canvas-sections-api
  description: Mark submission as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/assignments/assignment_id/submissions/{user_id}/read
  tags: Sections,Section,Id,Assignments,Assignment,Id,Submissions,User,Id,Read
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idread-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idassignmentsassignment-idsubmissionsuser-idread-put-openapi.md
- name: Instructure Canvas Sections API List enrollments
  x-api-slug: instructure-canvas-sections-api
  description: List enrollments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/enrollments
  tags: Sections,Section,Id,Enrollments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idenrollments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idenrollments-get-openapi.md
- name: Instructure Canvas Sections API Enroll a user
  x-api-slug: instructure-canvas-sections-api
  description: Enroll a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/enrollments
  tags: Sections,Section,Id,Enrollments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idenrollments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idenrollments-post-openapi.md
- name: Instructure Canvas Sections API List submissions for multiple assignments
  x-api-slug: instructure-canvas-sections-api
  description: List submissions for multiple assignments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/students/submissions
  tags: Sections,Section,Id,Students,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idstudentssubmissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idstudentssubmissions-get-openapi.md
- name: Instructure Canvas Sections API Grade or comment on multiple submissions
  x-api-slug: instructure-canvas-sections-api
  description: Grade or comment on multiple submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//sections/{section_id}/submissions/update_grades
  tags: Sections,Section,Id,Submissions,Update,Grades
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idsubmissionsupdate-grades-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/sectionssection-idsubmissionsupdate-grades-post-openapi.md
- name: Instructure Canvas Sections API
  x-api-slug: instructure-canvas-sections-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Users API List the activity stream
  x-api-slug: instructure-canvas-users-api
  description: List the activity stream.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/activity_stream
  tags: Users,Activity,Stream
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersactivity-stream-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersactivity-stream-get-openapi.md
- name: Instructure Canvas Users API Hide all stream items
  x-api-slug: instructure-canvas-users-api
  description: Hide all stream items.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/activity_stream
  tags: Users,Self,Activity,Stream
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfactivity-stream-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfactivity-stream-delete-openapi.md
- name: Instructure Canvas Users API List the activity stream
  x-api-slug: instructure-canvas-users-api
  description: List the activity stream.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/activity_stream
  tags: Users,Self,Activity,Stream
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfactivity-stream-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfactivity-stream-get-openapi.md
- name: Instructure Canvas Users API Activity stream summary
  x-api-slug: instructure-canvas-users-api
  description: Activity stream summary.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/activity_stream/summary
  tags: Users,Self,Activity,Stream,Summary
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfactivity-streamsummary-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfactivity-streamsummary-get-openapi.md
- name: Instructure Canvas Users API Hide a stream item
  x-api-slug: instructure-canvas-users-api
  description: Hide a stream item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/activity_stream/{id}
  tags: Users,Self,Activity,Stream,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfactivity-streamid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfactivity-streamid-delete-openapi.md
- name: Instructure Canvas Users API List bookmarks
  x-api-slug: instructure-canvas-users-api
  description: List bookmarks.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks
  tags: Users,Self,Bookmarks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarks-get-openapi.md
- name: Instructure Canvas Users API Create bookmark
  x-api-slug: instructure-canvas-users-api
  description: Create bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks
  tags: Users,Self,Bookmarks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarks-post-openapi.md
- name: Instructure Canvas Users API Delete bookmark
  x-api-slug: instructure-canvas-users-api
  description: Delete bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks/{id}
  tags: Users,Self,Bookmarks,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarksid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarksid-delete-openapi.md
- name: Instructure Canvas Users API Get bookmark
  x-api-slug: instructure-canvas-users-api
  description: Get bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks/{id}
  tags: Users,Self,Bookmarks,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarksid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarksid-get-openapi.md
- name: Instructure Canvas Users API Update bookmark
  x-api-slug: instructure-canvas-users-api
  description: Update bookmark.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/bookmarks/{id}
  tags: Users,Self,Bookmarks,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarksid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfbookmarksid-put-openapi.md
- name: Instructure Canvas Users API Update multiple preferences
  x-api-slug: instructure-canvas-users-api
  description: Update multiple preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{communication_channel_id}/notification_preferences
  tags: Users,Self,Communication,Channels,Communication,Channel,Id,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferences-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferences-put-openapi.md
- name: Instructure Canvas Users API Update a preference
  x-api-slug: instructure-canvas-users-api
  description: Update a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{communication_channel_id}/notification_preferences/notification
  tags: Users,Self,Communication,Channels,Communication,Channel,Id,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put-openapi.md
- name: Instructure Canvas Users API Update preferences by category
  x-api-slug: instructure-canvas-users-api
  description: Update preferences by category.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{communication_channel_id}/notification_preference_categories/category
  tags: Users,Self,Communication,Channels,Communication,Channel,Id,Notification,Preference,Categories,Category
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preference-categoriescategory-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelscommunication-channel-idnotification-preference-categoriescategory-put-openapi.md
- name: Instructure Canvas Users API Update multiple preferences
  x-api-slug: instructure-canvas-users-api
  description: Update multiple preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{type}/address/notification_preferences
  tags: Users,Self,Communication,Channels,Type,Address,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferences-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferences-put-openapi.md
- name: Instructure Canvas Users API Update a preference
  x-api-slug: instructure-canvas-users-api
  description: Update a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/communication_channels/{type}/address/notification_preferences/{notification}
  tags: Users,Self,Communication,Channels,Type,Address,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put-openapi.md
- name: Instructure Canvas Users API Clear course nicknames
  x-api-slug: instructure-canvas-users-api
  description: Clear course nicknames.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames
  tags: Users,Self,Course,Nicknames
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknames-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknames-delete-openapi.md
- name: Instructure Canvas Users API List course nicknames
  x-api-slug: instructure-canvas-users-api
  description: List course nicknames.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames
  tags: Users,Self,Course,Nicknames
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknames-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknames-get-openapi.md
- name: Instructure Canvas Users API Remove course nickname
  x-api-slug: instructure-canvas-users-api
  description: Remove course nickname.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames/{course_id}
  tags: Users,Self,Course,Nicknames,Course,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknamescourse-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknamescourse-id-delete-openapi.md
- name: Instructure Canvas Users API Get course nickname
  x-api-slug: instructure-canvas-users-api
  description: Get course nickname.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames/{course_id}
  tags: Users,Self,Course,Nicknames,Course,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknamescourse-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknamescourse-id-get-openapi.md
- name: Instructure Canvas Users API Set course nickname
  x-api-slug: instructure-canvas-users-api
  description: Set course nickname.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/course_nicknames/{course_id}
  tags: Users,Self,Course,Nicknames,Course,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknamescourse-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfcourse-nicknamescourse-id-put-openapi.md
- name: Instructure Canvas Users API Reset course favorites
  x-api-slug: instructure-canvas-users-api
  description: Reset course favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/courses
  tags: Users,Self,Favorites,Courses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritescourses-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritescourses-delete-openapi.md
- name: Instructure Canvas Users API List favorite courses
  x-api-slug: instructure-canvas-users-api
  description: List favorite courses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/courses
  tags: Users,Self,Favorites,Courses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritescourses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritescourses-get-openapi.md
- name: Instructure Canvas Users API Remove course from favorites
  x-api-slug: instructure-canvas-users-api
  description: Remove course from favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/courses/{id}
  tags: Users,Self,Favorites,Courses,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritescoursesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritescoursesid-delete-openapi.md
- name: Instructure Canvas Users API Add course to favorites
  x-api-slug: instructure-canvas-users-api
  description: Add course to favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/courses/{id}
  tags: Users,Self,Favorites,Courses,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritescoursesid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritescoursesid-post-openapi.md
- name: Instructure Canvas Users API Reset group favorites
  x-api-slug: instructure-canvas-users-api
  description: Reset group favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups
  tags: Users,Self,Favorites,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritesgroups-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritesgroups-delete-openapi.md
- name: Instructure Canvas Users API List favorite groups
  x-api-slug: instructure-canvas-users-api
  description: List favorite groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups
  tags: Users,Self,Favorites,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritesgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritesgroups-get-openapi.md
- name: Instructure Canvas Users API Remove group from favorites
  x-api-slug: instructure-canvas-users-api
  description: Remove group from favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups/{id}
  tags: Users,Self,Favorites,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritesgroupsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritesgroupsid-delete-openapi.md
- name: Instructure Canvas Users API Add group to favorites
  x-api-slug: instructure-canvas-users-api
  description: Add group to favorites.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/favorites/groups/{id}
  tags: Users,Self,Favorites,Groups,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritesgroupsid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselffavoritesgroupsid-post-openapi.md
- name: Instructure Canvas Users API List your groups
  x-api-slug: instructure-canvas-users-api
  description: List your groups.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/groups
  tags: Users,Self,Groups
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfgroups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfgroups-get-openapi.md
- name: Instructure Canvas Users API List the TODO items
  x-api-slug: instructure-canvas-users-api
  description: List the todo items.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/todo
  tags: Users,Self,Todo
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselftodo-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselftodo-get-openapi.md
- name: Instructure Canvas Users API List upcoming assignments, calendar events
  x-api-slug: instructure-canvas-users-api
  description: List upcoming assignments, calendar events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/upcoming_events
  tags: Users,Self,Upcoming,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfupcoming-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersselfupcoming-events-get-openapi.md
- name: Instructure Canvas Users API Show user details
  x-api-slug: instructure-canvas-users-api
  description: Show user details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}
  tags: Users,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersid-get-openapi.md
- name: Instructure Canvas Users API Edit a user
  x-api-slug: instructure-canvas-users-api
  description: Edit a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}
  tags: Users,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersid-put-openapi.md
- name: Instructure Canvas Users API Get custom colors
  x-api-slug: instructure-canvas-users-api
  description: Get custom colors.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/colors
  tags: Users,Id,Colors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidcolors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidcolors-get-openapi.md
- name: Instructure Canvas Users API Get custom color
  x-api-slug: instructure-canvas-users-api
  description: Get custom color.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/colors/asset_string
  tags: Users,Id,Colors,Asset,String
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidcolorsasset-string-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidcolorsasset-string-get-openapi.md
- name: Instructure Canvas Users API Update custom color
  x-api-slug: instructure-canvas-users-api
  description: Update custom color.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/colors/asset_string
  tags: Users,Id,Colors,Asset,String
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidcolorsasset-string-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidcolorsasset-string-put-openapi.md
- name: Instructure Canvas Users API Merge user into another user
  x-api-slug: instructure-canvas-users-api
  description: Merge user into another user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/merge_into/accounts/destination_account_id/users/{destination_user_id}
  tags: Users,Id,Merge,Into,Accounts,Destination,Account,Id,Users,Destination,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidmerge-intoaccountsdestination-account-idusersdestination-user-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidmerge-intoaccountsdestination-account-idusersdestination-user-id-put-openapi.md
- name: Instructure Canvas Users API Merge user into another user
  x-api-slug: instructure-canvas-users-api
  description: Merge user into another user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/merge_into/destination_user_id
  tags: Users,Id,Merge,Into,Destination,User,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidmerge-intodestination-user-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidmerge-intodestination-user-id-put-openapi.md
- name: Instructure Canvas Users API Update user settings.
  x-api-slug: instructure-canvas-users-api
  description: Update user settings..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/settings
  tags: Users,Id,Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidsettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidsettings-get-openapi.md
- name: Instructure Canvas Users API Update user settings.
  x-api-slug: instructure-canvas-users-api
  description: Update user settings..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{id}/settings
  tags: Users,Id,Settings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidsettings-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersidsettings-put-openapi.md
- name: Instructure Canvas Users API List avatar options
  x-api-slug: instructure-canvas-users-api
  description: List avatar options.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/avatars
  tags: Users,User,Id,Avatars
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idavatars-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idavatars-get-openapi.md
- name: Instructure Canvas Users API List calendar events for a user
  x-api-slug: instructure-canvas-users-api
  description: List calendar events for a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/calendar_events
  tags: Users,User,Id,Calendar,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcalendar-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcalendar-events-get-openapi.md
- name: Instructure Canvas Users API List user communication channels
  x-api-slug: instructure-canvas-users-api
  description: List user communication channels.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels
  tags: Users,User,Id,Communication,Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channels-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channels-get-openapi.md
- name: Instructure Canvas Users API Create a communication channel
  x-api-slug: instructure-canvas-users-api
  description: Create a communication channel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels
  tags: Users,User,Id,Communication,Channels
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channels-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channels-post-openapi.md
- name: Instructure Canvas Users API List preferences
  x-api-slug: instructure-canvas-users-api
  description: List preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/communication_channel_id/notification_preferences
  tags: Users,User,Id,Communication,Channels,Communication,Channel,Id,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferences-get-openapi.md
- name: Instructure Canvas Users API Get a preference
  x-api-slug: instructure-canvas-users-api
  description: Get a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/communication_channel_id/notification_preferences/{notification}
  tags: Users,User,Id,Communication,Channels,Communication,Channel,Id,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferencesnotification-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preferencesnotification-get-openapi.md
- name: Instructure Canvas Users API List of preference categories
  x-api-slug: instructure-canvas-users-api
  description: List of preference categories.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/communication_channel_id/notification_preference_categories
  tags: Users,User,Id,Communication,Channels,Communication,Channel,Id,Notification,Preference,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preference-categories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelscommunication-channel-idnotification-preference-categories-get-openapi.md
- name: Instructure Canvas Users API Delete a communication channel
  x-api-slug: instructure-canvas-users-api
  description: Delete a communication channel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/id
  tags: Users,User,Id,Communication,Channels,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelsid-delete-openapi.md
- name: Instructure Canvas Users API Delete a communication channel
  x-api-slug: instructure-canvas-users-api
  description: Delete a communication channel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/type/{address}
  tags: Users,User,Id,Communication,Channels,Type,Address
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelstypeaddress-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelstypeaddress-delete-openapi.md
- name: Instructure Canvas Users API List preferences
  x-api-slug: instructure-canvas-users-api
  description: List preferences.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/type/{address}/notification_preferences
  tags: Users,User,Id,Communication,Channels,Type,Address,Notification,Preferences
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferences-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferences-get-openapi.md
- name: Instructure Canvas Users API Get a preference
  x-api-slug: instructure-canvas-users-api
  description: Get a preference.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/communication_channels/type/{address}/notification_preferences/notification
  tags: Users,User,Id,Communication,Channels,Type,Address,Notification,Preferences,Notification
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferencesnotification-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcommunication-channelstypeaddressnotification-preferencesnotification-get-openapi.md
- name: Instructure Canvas Users API List content exports
  x-api-slug: instructure-canvas-users-api
  description: List content exports.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_exports
  tags: Users,User,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-exports-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-exports-get-openapi.md
- name: Instructure Canvas Users API Export content
  x-api-slug: instructure-canvas-users-api
  description: Export content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_exports
  tags: Users,User,Id,Content,Exports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-exports-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-exports-post-openapi.md
- name: Instructure Canvas Users API Show content export
  x-api-slug: instructure-canvas-users-api
  description: Show content export.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_exports/id
  tags: Users,User,Id,Content,Exports,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-exportsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-exportsid-get-openapi.md
- name: Instructure Canvas Users API List licenses
  x-api-slug: instructure-canvas-users-api
  description: List licenses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_licenses
  tags: Users,User,Id,Content,Licenses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-licenses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-licenses-get-openapi.md
- name: Instructure Canvas Users API List content migrations
  x-api-slug: instructure-canvas-users-api
  description: List content migrations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations
  tags: Users,User,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrations-get-openapi.md
- name: Instructure Canvas Users API Create a content migration
  x-api-slug: instructure-canvas-users-api
  description: Create a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations
  tags: Users,User,Id,Content,Migrations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrations-post-openapi.md
- name: Instructure Canvas Users API List migration issues
  x-api-slug: instructure-canvas-users-api
  description: List migration issues.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/content_migration_id/migration_issues
  tags: Users,User,Id,Content,Migrations,Content,Migration,Id,Migration,Issues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issues-get-openapi.md
- name: Instructure Canvas Users API Get a migration issue
  x-api-slug: instructure-canvas-users-api
  description: Get a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Users,User,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-get-openapi.md
- name: Instructure Canvas Users API Update a migration issue
  x-api-slug: instructure-canvas-users-api
  description: Update a migration issue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/content_migration_id/migration_issues/{id}
  tags: Users,User,Id,Content,Migrations,Content,Migration,Id,Migration,Issues,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-put-openapi.md
- name: Instructure Canvas Users API Get a content migration
  x-api-slug: instructure-canvas-users-api
  description: Get a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/id
  tags: Users,User,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationsid-get-openapi.md
- name: Instructure Canvas Users API Update a content migration
  x-api-slug: instructure-canvas-users-api
  description: Update a content migration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/id
  tags: Users,User,Id,Content,Migrations,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationsid-put-openapi.md
- name: Instructure Canvas Users API List Migration Systems
  x-api-slug: instructure-canvas-users-api
  description: List migration systems.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/content_migrations/migrators
  tags: Users,User,Id,Content,Migrations,Migrators
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationsmigrators-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcontent-migrationsmigrators-get-openapi.md
- name: Instructure Canvas Users API List courses for a user
  x-api-slug: instructure-canvas-users-api
  description: List courses for a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/courses
  tags: Users,User,Id,Courses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcourses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcourses-get-openapi.md
- name: Instructure Canvas Users API List assignments for user
  x-api-slug: instructure-canvas-users-api
  description: List assignments for user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/courses/course_id/assignments
  tags: Users,User,Id,Courses,Course,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcoursescourse-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcoursescourse-idassignments-get-openapi.md
- name: Instructure Canvas Users API Delete custom data
  x-api-slug: instructure-canvas-users-api
  description: Delete custom data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/custom_data(/*scope)
  tags: Users,User,Id,Custom,Data(,*scope)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcustom-datascope-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcustom-datascope-delete-openapi.md
- name: Instructure Canvas Users API Load custom data
  x-api-slug: instructure-canvas-users-api
  description: Load custom data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/custom_data(/*scope)
  tags: Users,User,Id,Custom,Data(,*scope)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcustom-datascope-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcustom-datascope-get-openapi.md
- name: Instructure Canvas Users API Store custom data
  x-api-slug: instructure-canvas-users-api
  description: Store custom data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/custom_data(/*scope)
  tags: Users,User,Id,Custom,Data(,*scope)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcustom-datascope-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idcustom-datascope-put-openapi.md
- name: Instructure Canvas Users API List enrollments
  x-api-slug: instructure-canvas-users-api
  description: List enrollments.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/enrollments
  tags: Users,User,Id,Enrollments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idenrollments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idenrollments-get-openapi.md
- name: Instructure Canvas Users API List features
  x-api-slug: instructure-canvas-users-api
  description: List features.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features
  tags: Users,User,Id,Features
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeatures-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeatures-get-openapi.md
- name: Instructure Canvas Users API List enabled features
  x-api-slug: instructure-canvas-users-api
  description: List enabled features.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features/enabled
  tags: Users,User,Id,Features,Enabled
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeaturesenabled-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeaturesenabled-get-openapi.md
- name: Instructure Canvas Users API Remove feature flag
  x-api-slug: instructure-canvas-users-api
  description: Remove feature flag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features/flags/feature
  tags: Users,User,Id,Features,Flags,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeaturesflagsfeature-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeaturesflagsfeature-delete-openapi.md
- name: Instructure Canvas Users API Get feature flag
  x-api-slug: instructure-canvas-users-api
  description: Get feature flag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features/flags/feature
  tags: Users,User,Id,Features,Flags,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeaturesflagsfeature-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeaturesflagsfeature-get-openapi.md
- name: Instructure Canvas Users API Set feature flag
  x-api-slug: instructure-canvas-users-api
  description: Set feature flag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/features/flags/feature
  tags: Users,User,Id,Features,Flags,Feature
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeaturesflagsfeature-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfeaturesflagsfeature-put-openapi.md
- name: Instructure Canvas Users API List files
  x-api-slug: instructure-canvas-users-api
  description: List files.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/files
  tags: Users,User,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfiles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfiles-get-openapi.md
- name: Instructure Canvas Users API Upload a file
  x-api-slug: instructure-canvas-users-api
  description: Upload a file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/files
  tags: Users,User,Id,Files
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfiles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfiles-post-openapi.md
- name: Instructure Canvas Users API Get file
  x-api-slug: instructure-canvas-users-api
  description: Get file.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/files/id
  tags: Users,User,Id,Files,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfilesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfilesid-get-openapi.md
- name: Instructure Canvas Users API Get quota information
  x-api-slug: instructure-canvas-users-api
  description: Get quota information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/files/quota
  tags: Users,User,Id,Files,Quota
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfilesquota-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfilesquota-get-openapi.md
- name: Instructure Canvas Users API List all folders
  x-api-slug: instructure-canvas-users-api
  description: List all folders.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders
  tags: Users,User,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfolders-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfolders-get-openapi.md
- name: Instructure Canvas Users API Create folder
  x-api-slug: instructure-canvas-users-api
  description: Create folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders
  tags: Users,User,Id,Folders
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfolders-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfolders-post-openapi.md
- name: Instructure Canvas Users API Resolve path
  x-api-slug: instructure-canvas-users-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders/by_path
  tags: Users,User,Id,Folders,By,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfoldersby-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfoldersby-path-get-openapi.md
- name: Instructure Canvas Users API Resolve path
  x-api-slug: instructure-canvas-users-api
  description: Resolve path.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders/by_path/*full_path
  tags: Users,User,Id,Folders,By,Path,*full,Path
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfoldersby-pathfull-path-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfoldersby-pathfull-path-get-openapi.md
- name: Instructure Canvas Users API Get folder
  x-api-slug: instructure-canvas-users-api
  description: Get folder.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/folders/id
  tags: Users,User,Id,Folders,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfoldersid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idfoldersid-get-openapi.md
- name: Instructure Canvas Users API List user logins
  x-api-slug: instructure-canvas-users-api
  description: List user logins.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/logins
  tags: Users,User,Id,Logins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idlogins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idlogins-get-openapi.md
- name: Instructure Canvas Users API Delete a user login
  x-api-slug: instructure-canvas-users-api
  description: Delete a user login.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/logins/id
  tags: Users,User,Id,Logins,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idloginsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idloginsid-delete-openapi.md
- name: Instructure Canvas Users API List Missing Submissions
  x-api-slug: instructure-canvas-users-api
  description: List missing submissions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/missing_submissions
  tags: Users,User,Id,Missing,Submissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idmissing-submissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idmissing-submissions-get-openapi.md
- name: Instructure Canvas Users API List observees
  x-api-slug: instructure-canvas-users-api
  description: List observees.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees
  tags: Users,User,Id,Observees
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobservees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobservees-get-openapi.md
- name: Instructure Canvas Users API Add an observee with credentials
  x-api-slug: instructure-canvas-users-api
  description: Add an observee with credentials.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees
  tags: Users,User,Id,Observees
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobservees-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobservees-post-openapi.md
- name: Instructure Canvas Users API Remove an observee
  x-api-slug: instructure-canvas-users-api
  description: Remove an observee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees/observee_id
  tags: Users,User,Id,Observees,Observee,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobserveesobservee-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobserveesobservee-id-delete-openapi.md
- name: Instructure Canvas Users API Show an observee
  x-api-slug: instructure-canvas-users-api
  description: Show an observee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees/observee_id
  tags: Users,User,Id,Observees,Observee,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobserveesobservee-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobserveesobservee-id-get-openapi.md
- name: Instructure Canvas Users API Add an observee
  x-api-slug: instructure-canvas-users-api
  description: Add an observee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/observees/observee_id
  tags: Users,User,Id,Observees,Observee,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobserveesobservee-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idobserveesobservee-id-put-openapi.md
- name: Instructure Canvas Users API List user page views
  x-api-slug: instructure-canvas-users-api
  description: List user page views.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/page_views
  tags: Users,User,Id,Page,Views
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idpage-views-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idpage-views-get-openapi.md
- name: Instructure Canvas Users API Get user profile
  x-api-slug: instructure-canvas-users-api
  description: Get user profile.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/profile
  tags: Users,User,Id,Profile
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idprofile-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idprofile-get-openapi.md
- name: Instructure Canvas Users API Remove usage rights
  x-api-slug: instructure-canvas-users-api
  description: Remove usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/usage_rights
  tags: Users,User,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idusage-rights-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idusage-rights-delete-openapi.md
- name: Instructure Canvas Users API Set usage rights
  x-api-slug: instructure-canvas-users-api
  description: Set usage rights.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/usage_rights
  tags: Users,User,Id,Usage,Rights
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idusage-rights-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/usersuser-idusage-rights-put-openapi.md
- name: Instructure Canvas Users API
  x-api-slug: instructure-canvas-users-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
- name: Instructure Canvas Utility APIs Retrieve assignments enabled for grade export
    to SIS
  x-api-slug: instructure-canvas-utility-apis
  description: Retrieve assignments enabled for grade export to sis.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//api/sis/accounts/{account_id}/assignments
  tags: Api,Sis,Accounts,Account,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/apisisaccountsaccount-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/apisisaccountsaccount-idassignments-get-openapi.md
- name: Instructure Canvas Utility APIs Retrieve assignments enabled for grade export
    to SIS
  x-api-slug: instructure-canvas-utility-apis
  description: Retrieve assignments enabled for grade export to sis.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//api/sis/courses/{course_id}/assignments
  tags: Api,Sis,Courses,Course,Id,Assignments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/apisiscoursescourse-idassignments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/apisiscoursescourse-idassignments-get-openapi.md
- name: Instructure Canvas Utility APIs List members of a collaboration.
  x-api-slug: instructure-canvas-utility-apis
  description: List members of a collaboration..
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//collaborations/{id}/members
  tags: Collaborations,Id,Members
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/collaborationsidmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/collaborationsidmembers-get-openapi.md
- name: Instructure Canvas Utility APIs List of CommMessages for a user
  x-api-slug: instructure-canvas-utility-apis
  description: List of commmessages for a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//comm_messages
  tags: Comm,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/comm-messages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/comm-messages-get-openapi.md
- name: Instructure Canvas Utility APIs List accounts for course admins
  x-api-slug: instructure-canvas-utility-apis
  description: List accounts for course admins.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//course_accounts
  tags: Course,Accounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/course-accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/course-accounts-get-openapi.md
- name: Instructure Canvas Utility APIs Create Error Report
  x-api-slug: instructure-canvas-utility-apis
  description: Create error report.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//error_reports
  tags: Error,Reports
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/error-reports-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/error-reports-post-openapi.md
- name: Instructure Canvas Utility APIs Create JWT
  x-api-slug: instructure-canvas-utility-apis
  description: Create jwt.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//jwts
  tags: Jwts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/jwts-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/jwts-post-openapi.md
- name: Instructure Canvas Utility APIs Show an outcome
  x-api-slug: instructure-canvas-utility-apis
  description: Show an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//outcomes/{id}
  tags: Outcomes,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/outcomesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/outcomesid-get-openapi.md
- name: Instructure Canvas Utility APIs Update an outcome
  x-api-slug: instructure-canvas-utility-apis
  description: Update an outcome.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//outcomes/{id}
  tags: Outcomes,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/outcomesid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/outcomesid-put-openapi.md
- name: Instructure Canvas Utility APIs Query progress
  x-api-slug: instructure-canvas-utility-apis
  description: Query progress.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//progress/{id}
  tags: Progress,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/progressid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/progressid-get-openapi.md
- name: Instructure Canvas Utility APIs List all courses
  x-api-slug: instructure-canvas-utility-apis
  description: List all courses.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//search/all_courses
  tags: Search,,Courses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/searchall-courses-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/searchall-courses-get-openapi.md
- name: Instructure Canvas Utility APIs Find recipients
  x-api-slug: instructure-canvas-utility-apis
  description: Find recipients.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//search/recipients
  tags: Search,Recipients
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/searchrecipients-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/searchrecipients-get-openapi.md
- name: Instructure Canvas Utility APIs Get Kaltura config
  x-api-slug: instructure-canvas-utility-apis
  description: Get kaltura config.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//services/kaltura
  tags: Services,Kaltura
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/serviceskaltura-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/serviceskaltura-get-openapi.md
- name: Instructure Canvas Utility APIs Start Kaltura session
  x-api-slug: instructure-canvas-utility-apis
  description: Start kaltura session.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//services/kaltura_session
  tags: Services,Kaltura,Session
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/serviceskaltura-session-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/serviceskaltura-session-post-openapi.md
- name: Instructure Canvas Utility APIs
  x-api-slug: instructure-canvas-utility-apis
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Instructure
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/instructure/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---