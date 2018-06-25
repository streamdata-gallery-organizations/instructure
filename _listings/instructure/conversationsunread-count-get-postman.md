{
  "info": {
    "name": "Instructure Canvas Conversations API Unread count",
    "_postman_id": "d4886044-2964-4ba1-bd23-6e5bfaadfba9",
    "description": "Unread count.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "bc02eeba-0e25-4f69-afab-ea89fc7cf88f",
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
              "id": "7cf3a731-71bc-4937-97a5-f82d156a0ea2"
            }
          ]
        },
        {
          "id": "f3b7ba29-363c-4b4a-8e0a-1b46a730aacf",
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
              "id": "b67c8413-36cd-4c95-bbd1-c1a60c6a5dbe"
            }
          ]
        },
        {
          "id": "9826a792-107c-4c1c-83d1-028103331a06",
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
              "id": "7afce716-b610-49a2-8fdf-62461e0ec81e"
            }
          ]
        },
        {
          "id": "05283f38-dc9d-40f8-8bef-34949dd0db70",
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
              "id": "82e5de72-0490-4ba7-bc60-2660a392e1d5"
            }
          ]
        },
        {
          "id": "a3f00f4e-55e9-4e03-88cc-8c6d8f1daf34",
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
              "id": "2dabc993-14d2-47f5-a91f-3788a9f7f138"
            }
          ]
        },
        {
          "id": "475953c8-23f0-4e75-8baf-a05b4bb507e8",
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
              "id": "c0e22729-18f1-4e1b-a076-007da98c9612"
            }
          ]
        },
        {
          "id": "5211334c-3e2a-410c-b661-f3d32bf8d63d",
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
              "id": "02e43cc0-6f85-4366-8e14-0648f102546d"
            }
          ]
        }
      ]
    }
  ]
}