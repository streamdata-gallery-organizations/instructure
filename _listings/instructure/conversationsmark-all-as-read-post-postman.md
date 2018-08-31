{
  "info": {
    "name": "Instructure Canvas Conversations API Mark all as read",
    "_postman_id": "8e1a05d7-d7fa-45fa-a05a-9284e3903884",
    "description": "Mark all as read.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "23142e96-9d00-4209-87fc-30be6d896eaa",
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
              "id": "c47ae3dd-1fee-44f5-b71e-0122b537905a"
            }
          ]
        },
        {
          "id": "d7be13ca-9b29-4324-9acc-7005147aaff0",
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
              "id": "8e05a575-9758-4170-bbfd-d1e0fbd09f79"
            }
          ]
        },
        {
          "id": "fc00115c-6927-499c-b3bb-fe2a7e14c96d",
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
              "id": "c63afca9-5349-4616-ad4c-8e9ac0fe5f98"
            }
          ]
        },
        {
          "id": "147aa02a-d9e7-4a54-9349-8dfcfee75e4c",
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
              "id": "acdd8d33-70cd-45bd-9448-8ed880a7f04f"
            }
          ]
        },
        {
          "id": "4396416f-22d3-40db-bd5d-1821d4e57178",
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
              "id": "db780054-4160-4089-91cf-5eeda0581d25"
            }
          ]
        },
        {
          "id": "758db243-4348-44bb-8c2d-f69da9d7b418",
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
              "id": "8decf222-397b-4818-86e3-501b14b10a99"
            }
          ]
        }
      ]
    }
  ]
}