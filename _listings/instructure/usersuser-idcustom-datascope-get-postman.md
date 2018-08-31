{
  "info": {
    "name": "Instructure Canvas Users API Load custom data",
    "_postman_id": "e3db65db-1d82-40de-959a-6f03530e0e4c",
    "description": "Load custom data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "947fc932-48c9-4aa4-8e91-11ca49bef0f6",
          "name": "load-custom-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/custom_data(/*scope)"
              ],
              "query": [
                {
                  "key": "ns",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Load custom data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dabd8c02-0517-49ec-b3a1-89d4de85bb40"
            }
          ]
        },
        {
          "id": "3887a5c7-b62d-40bf-bd37-112e9dc3a397",
          "name": "delete-custom-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/custom_data(/*scope)"
              ],
              "query": [
                {
                  "key": "ns",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete custom data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92114a50-d4fb-4de0-a2a7-501b0e5c5fac"
            }
          ]
        }
      ]
    }
  ]
}