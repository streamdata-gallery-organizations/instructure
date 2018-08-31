{
  "info": {
    "name": "Instructure Canvas Conversations API Edit a conversation",
    "_postman_id": "3de005af-a895-4946-8164-295eed7dc6c8",
    "description": "Edit a conversation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "2337ccdd-5bcb-4e3f-99ce-ce2c70792066",
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
              "id": "4404cd59-c7d9-4d95-8e32-3f769f93dd91"
            }
          ]
        },
        {
          "id": "4b4d32b3-e0df-49ba-95bb-5e78bf5193d1",
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
              "id": "7d4de2ba-1c5f-4139-8540-ac9719ba5f72"
            }
          ]
        },
        {
          "id": "7b85190c-5d59-4a49-a490-6e6c530ff152",
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
              "id": "2bba4830-108c-4f11-86a7-4ba9c112a6ad"
            }
          ]
        },
        {
          "id": "4c10d3e2-3702-4931-a8c6-69f9c9543fcd",
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
              "id": "c8d0bf40-aad2-49dd-8e1e-16fc5984b5a0"
            }
          ]
        },
        {
          "id": "c6e3ca7a-0c72-430c-a506-08f0de2e8fe6",
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
              "id": "15fc3978-b9ea-4b10-b80d-119aa8e60198"
            }
          ]
        },
        {
          "id": "f01adb24-6772-4c66-a096-008289ae83bb",
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
              "id": "8820065d-5f06-4ad0-b8da-c3e9a14fabfe"
            }
          ]
        },
        {
          "id": "4564f714-a16b-4872-96b0-78ab85345d6c",
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
              "id": "1ec2d518-3536-4ff4-a99f-a296b270e38a"
            }
          ]
        },
        {
          "id": "c0ce425e-0ad6-485f-abff-5a2f4118fc7e",
          "name": "get-a-single-conversation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "conversations/:id"
              ],
              "query": [
                {
                  "key": "auto_mark_as_read",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "filter",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "filter_mode",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "interleave_submissions",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "scope",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single conversation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aefd160a-e633-4b28-9a4b-ca0b30af8d75"
            }
          ]
        },
        {
          "id": "099a9b84-69c9-414f-b99b-cc381e49bfa6",
          "name": "edit-a-conversation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "conversations/:id"
              ],
              "query": [
                {
                  "key": "conversation[starred]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "conversation[subject]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "conversation[subscribed]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "conversation[workflow_state]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "filter",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "filter_mode",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "scope",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a conversation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b5ab4e5-14d6-486a-b199-200d0581233a"
            }
          ]
        },
        {
          "id": "693207dc-14d6-4dcc-a0f0-e68edc42663c",
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
              "id": "216faa9d-c9c9-456c-a20d-78f632b18af3"
            }
          ]
        }
      ]
    }
  ]
}