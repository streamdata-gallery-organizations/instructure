{
  "info": {
    "name": "Instructure Canvas Conversations API Get a single conversation",
    "_postman_id": "1ca178a1-3c6b-4667-b4af-d2d8334776c8",
    "description": "Get a single conversation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "f3ae39d8-9fda-46d1-a20c-bd699d42deb8",
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
              "id": "8650bb26-79ca-4d67-9c5c-3cb38e359118"
            }
          ]
        },
        {
          "id": "7a9c997c-22ce-4333-a40a-b947ce752774",
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
              "id": "5e212c6d-9836-425c-b34d-1241f42cbc1c"
            }
          ]
        },
        {
          "id": "899d2741-87ee-4825-ae36-fe773bee7e5a",
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
              "id": "2539dae8-eca0-489d-a4fb-19e62361e25f"
            }
          ]
        },
        {
          "id": "fbb8487f-edc5-448e-bccb-ef76276823b2",
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
              "id": "db34ad52-3f15-47cd-a1f3-43aa40482eee"
            }
          ]
        },
        {
          "id": "2882078d-3fd7-47ba-a5fd-4c4e0a1d582d",
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
              "id": "16045c6f-2766-456b-9db6-5de9f1a97cbb"
            }
          ]
        },
        {
          "id": "ee9a47e4-ddd3-45f8-a0c4-9e5e1416c755",
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
              "id": "b5ffaa59-ab22-4fb8-96b0-c52242bf61d8"
            }
          ]
        },
        {
          "id": "f4fba9c4-2b84-4aee-b80a-c197d159b75f",
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
              "id": "a8d185ef-8ab4-4114-8c3e-cf888761f867"
            }
          ]
        },
        {
          "id": "173621da-d4dd-4afb-b31f-dcc83b324e31",
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
              "id": "671a82f9-17f8-4f5f-b57b-d9b91124c0bc"
            }
          ]
        },
        {
          "id": "8bd1a51a-7bca-402e-a31c-adaaa31cba2c",
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
              "id": "3a6f0968-74e6-4758-ac12-4ab129c389b4"
            }
          ]
        }
      ]
    }
  ]
}