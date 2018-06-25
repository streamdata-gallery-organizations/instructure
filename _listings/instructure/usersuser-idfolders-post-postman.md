{
  "info": {
    "name": "Instructure Canvas Users API Create folder",
    "_postman_id": "e6958b0a-2ef9-4851-b689-a6e671b7ee0e",
    "description": "Create folder.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "fe942651-ee18-42b1-97dd-8379386f8cdd",
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
              "id": "4009c277-805a-48a1-895c-6c145c7efbfd"
            }
          ]
        },
        {
          "id": "f85ce75d-e333-4f2c-ab18-f4741f4a7f4b",
          "name": "create-folder",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/folders"
              ],
              "query": [
                {
                  "key": "hidden",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "locked",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "parent_folder_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "parent_folder_path",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "unlock_at",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create folder."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7315d139-96d2-4811-a987-eae416a69b3c"
            }
          ]
        }
      ]
    }
  ]
}