{
  "info": {
    "name": "Instructure Canvas Conversations API Delete a conversation",
    "_postman_id": "298e49ab-f252-412a-9198-f1d813480ef6",
    "description": "Delete a conversation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "7e71fe8b-e7e4-4c25-becf-fa38a7e39277",
          "name": "list-conversations",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/conversations?filter=%5B%7B%7D%5D&filter_mode=%7B%7D&include_all_conversation_ids=%7B%7D&interleave_submissions=%7B%7D&scope=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List conversations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80ed2cc7-4f0e-4a8a-b687-196ee926ba34"
            }
          ]
        },
        {
          "id": "517613bc-8a62-43d6-8f1b-ed5937a845bd",
          "name": "batch-update-conversations",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/conversations?conversation_ids=%5B%7B%7D%5D&event=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Batch update conversations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5501fda8-61ca-4413-8854-779db7020e64"
            }
          ]
        },
        {
          "id": "0a4ff8c6-a21e-4f75-890d-c232b5a004f4",
          "name": "create-a-conversation",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/conversations?attachment_ids=%5B%7B%7D%5D&body=%7B%7D&context_code=%7B%7D&filter=%5B%7B%7D%5D&filter_mode=%7B%7D&group_conversation=%7B%7D&media_comment_id=%7B%7D&media_comment_type=%7B%7D&mode=%7B%7D&recipients=%5B%7B%7D%5D&scope=%7B%7D&subject=%7B%7D&user_note=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a conversation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c64fb3b-5fbe-4372-8bb7-8027bbaa4412"
            }
          ]
        },
        {
          "id": "a956bb4a-f007-41fa-a00e-002718655702",
          "name": "get-running-batches",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/conversations/batches",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get running batches."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4168484-020f-4e94-acd8-f8a144805d22"
            }
          ]
        },
        {
          "id": "815761d2-2298-4776-827f-e2d3adebcb77",
          "name": "find-recipients",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/conversations/find_recipients?context=%7B%7D&exclude=%5B%7B%7D%5D&from_conversation_id=%7B%7D&permissions=%5B%7B%7D%5D&search=%7B%7D&type=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Find recipients."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a637ea0a-af56-43a6-9a8e-c9f3552da458"
            }
          ]
        },
        {
          "id": "31b7c829-881a-436f-bb1b-2cca31ed2a8a",
          "name": "mark-all-as-read",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/conversations/mark_all_as_read",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Mark all as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cde0cb9d-4d09-4c45-8389-b628a96e1265"
            }
          ]
        },
        {
          "id": "bc643951-c17c-43ba-8ecf-dd00f76c99e2",
          "name": "unread-count",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/conversations/unread_count",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Unread count."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d5d9cfad-f81b-42a3-8498-a797dd2ba1af"
            }
          ]
        },
        {
          "id": "9ea283f6-2e2b-4ff8-b753-a5d16f7abeb6",
          "name": "delete-a-conversation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "conversations/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a conversation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "280cf8c6-0312-4c58-97bc-741744d31d94"
            }
          ]
        }
      ]
    }
  ]
}