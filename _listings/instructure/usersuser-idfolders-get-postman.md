{
  "info": {
    "name": "Instructure Canvas Users API List all folders",
    "_postman_id": "e1a00b50-ad83-4a56-a44c-9c01ba56bb4f",
    "description": "List all folders.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "50c752cf-b6f9-40c1-b2a6-e8f79d2b5bf6",
          "name": "list-all-folders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/folders"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all folders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "406e141e-5d12-44a2-b378-d46b4fbecc9c"
            }
          ]
        }
      ]
    }
  ]
}