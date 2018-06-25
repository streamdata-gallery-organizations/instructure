---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Polls API List poll sessions for a poll
  description: List poll sessions for a poll.
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