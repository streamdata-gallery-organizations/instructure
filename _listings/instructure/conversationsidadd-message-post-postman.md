{
  "info": {
    "name": "Instructure Canvas Conversations API Add a message",
    "_postman_id": "20b2cd66-cca8-4563-a277-75d45fa02178",
    "description": "Add a message.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "b6485a79-c235-4906-9350-814280867aa2",
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
              "id": "4a477d01-4df6-453f-a776-ee39e7a1ff10"
            }
          ]
        },
        {
          "id": "7d225602-42d5-40b5-980e-d1dfe73d5953",
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
              "id": "150b5eee-2780-4168-9d00-7899964c8684"
            }
          ]
        },
        {
          "id": "b12344c8-ec36-4b99-a24a-9b6cfd0ad059",
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
              "id": "e6d17ded-216f-48b7-86f2-049ae3595f3c"
            }
          ]
        },
        {
          "id": "d4a1b1f6-7f31-4b4a-8cad-1ad7400350c3",
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
              "id": "72e8f441-2d08-4afe-93a2-aa73f6b97ef4"
            }
          ]
        },
        {
          "id": "9dd9ad38-0795-4022-9023-f409a07b9bb4",
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
              "id": "1079187c-080e-4b61-b8e7-b9882f5d316d"
            }
          ]
        },
        {
          "id": "ac44d429-d96c-417a-a060-6b708b63c987",
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
              "id": "3ed5b42f-e250-4b61-bb8d-6cf18b098e67"
            }
          ]
        },
        {
          "id": "9db3a9ab-3381-447e-8f89-ee01c7985780",
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
              "id": "e819007b-1814-4591-b98f-0d70f2759ee3"
            }
          ]
        },
        {
          "id": "c165aaba-dd75-4604-9fb7-d5b432599682",
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
              "id": "3514a7c4-96c6-4c6c-8ba4-8978f5462da1"
            }
          ]
        },
        {
          "id": "be03dc42-abe3-409d-a34d-90185de7dade",
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
              "id": "0c822ca6-c7a1-47e7-8457-dfea8e814e9a"
            }
          ]
        },
        {
          "id": "48b91a06-b68d-47a7-b5c3-6089ee7f79c7",
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
              "id": "96f5cffc-bbb1-4950-a632-68e57d234f62"
            }
          ]
        },
        {
          "id": "1c4c5122-3ec8-448b-92d4-94be35bdc892",
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
              "id": "12e5ad4e-4586-4a54-998c-2c4c9919ce12"
            }
          ]
        }
      ]
    }
  ]
}