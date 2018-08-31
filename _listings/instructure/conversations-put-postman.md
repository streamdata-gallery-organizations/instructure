{
  "info": {
    "name": "Instructure Canvas Conversations API Batch update conversations",
    "_postman_id": "f99d03e6-7f4a-46c7-b3f4-78c71669bf12",
    "description": "Batch update conversations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "c8acf252-b25f-4104-9319-99559bd1124a",
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
              "id": "53a1a45c-7177-4d1e-a45d-0cdb39b40080"
            }
          ]
        },
        {
          "id": "07edc752-4547-4622-9fe8-acce1f606de3",
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
              "id": "970eccec-eeac-4f70-9362-c65e7243207e"
            }
          ]
        },
        {
          "id": "0a6cf2c9-e5cd-4c21-bc75-0eccededb3be",
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
              "id": "b8283b6d-39ab-458c-9e28-f61c403fc13a"
            }
          ]
        }
      ]
    }
  ]
}