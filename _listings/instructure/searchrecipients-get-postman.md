{
  "info": {
    "name": "Instructure Canvas Utility APIs Find recipients",
    "_postman_id": "398fb226-aaae-44a6-927f-853cd2208dae",
    "description": "Find recipients.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Search",
      "item": [
        {
          "id": "545cb59c-d7d8-411a-81b4-33f8e3cbbf99",
          "name": "find-recipients",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/search/recipients?context=%7B%7D&exclude=%5B%7B%7D%5D&from_conversation_id=%7B%7D&permissions=%5B%7B%7D%5D&search=%7B%7D&type=%7B%7D&user_id=%7B%7D",
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
              "id": "ae772918-8796-4742-a74c-32ea209c1a7a"
            }
          ]
        }
      ]
    }
  ]
}