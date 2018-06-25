---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Conversations API Batch update conversations
  description: Batch update conversations.
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