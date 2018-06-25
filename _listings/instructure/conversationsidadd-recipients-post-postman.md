{
  "info": {
    "name": "Instructure Canvas Conversations API Add recipients",
    "_postman_id": "e8241273-1f27-40e7-ad89-0f00456fc049",
    "description": "Add recipients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "087b78a3-8d71-4c7c-a9e5-2b2b4dd3450d",
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
              "id": "047bd1de-80f3-402d-9876-82486ce05fb7"
            }
          ]
        },
        {
          "id": "dfe5d72f-fbd5-4ce8-9052-008533728d0d",
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
              "id": "0d8814ba-e3a4-4004-9d8a-9097a785238d"
            }
          ]
        },
        {
          "id": "5f6cd232-dc3c-4e01-9197-92483af60579",
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
              "id": "dd6b2103-656e-4a92-a31b-37db6bef9f03"
            }
          ]
        },
        {
          "id": "bc659eb3-3739-47d5-84d8-40ad882f1819",
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
              "id": "7f1f7369-bbc6-4385-af88-fbe20506b395"
            }
          ]
        },
        {
          "id": "dd27f6d0-4bb7-4948-be38-1b6eca4cb621",
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
              "id": "57d84adb-cae4-4586-81d9-001c2634f2d0"
            }
          ]
        },
        {
          "id": "4e2a0674-0fbe-4b90-9e33-5dcb58c248fd",
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
              "id": "2729fdad-9e56-4f47-901b-067f9b68f3ba"
            }
          ]
        },
        {
          "id": "b07fddda-6fb1-4420-85f7-7f6d03ef9f18",
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
              "id": "40e8af51-44ca-432f-bfd1-4c70ad94ca90"
            }
          ]
        },
        {
          "id": "18f8fa35-3347-48dd-87a7-9e312aa10ded",
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
              "id": "f5dd9c26-3c93-4e66-9e9f-3c7c91a1bb54"
            }
          ]
        },
        {
          "id": "88511d34-6e34-41dc-84a9-c9e7a382a526",
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
              "id": "44fb21fc-f123-4f26-baf3-a5947cc58336"
            }
          ]
        },
        {
          "id": "4a39739d-01b2-4728-ba71-706b4847fa4c",
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
              "id": "33ebe27c-8015-4714-ad66-ade313e62ed8"
            }
          ]
        },
        {
          "id": "4087bc8c-12d2-434f-a783-4c6916f6a5a6",
          "name": "add-a-message",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "conversations/:id/add_message"
              ],
              "query": [
                {
                  "key": "attachment_ids",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "body",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "included_messages",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "media_comment_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "media_comment_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "recipients",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "user_note",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c9e13b9-1b35-450a-b63a-4aad9546d8d3"
            }
          ]
        },
        {
          "id": "a5a459b6-c953-4a06-90a9-03010c0bfa00",
          "name": "add-recipients",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "conversations/:id/add_recipients"
              ],
              "query": [
                {
                  "key": "recipients",
                  "value": "%5B%7B%7D%5D",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add recipients."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73636010-0bc2-4ed4-be0d-3612d6bd5650"
            }
          ]
        }
      ]
    }
  ]
}