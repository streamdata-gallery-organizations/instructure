{
  "info": {
    "name": "Instructure Canvas Conversations API Get running batches",
    "_postman_id": "707d3bcf-e771-4ca6-8bdf-d764e4be0e7a",
    "description": "Get running batches.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Conversations",
      "item": [
        {
          "id": "188fc7d8-0e7a-4df2-8afa-5808c1a63946",
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
              "id": "bff0a537-bd3a-406c-8574-4b3bbf2cb4a1"
            }
          ]
        }
      ]
    }
  ]
}