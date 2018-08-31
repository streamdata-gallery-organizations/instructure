{
  "info": {
    "name": "Instructure Canvas Conversations API List conversations",
    "_postman_id": "faef190f-e3ae-4135-934c-3a293324f854",
    "description": "List conversations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "8084682a-8a21-4303-b88a-108742709a41",
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
              "id": "23b5b9dd-96b2-4397-ae32-a90391d0ac1f"
            }
          ]
        }
      ]
    }
  ]
}