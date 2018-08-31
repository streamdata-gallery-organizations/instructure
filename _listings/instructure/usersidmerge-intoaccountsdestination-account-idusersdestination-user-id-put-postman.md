{
  "info": {
    "name": "Instructure Canvas Users API Merge user into another user",
    "_postman_id": "fe8d9415-81c9-4607-ba02-854f1d53b9ec",
    "description": "Merge user into another user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "f9340b4a-d7d8-4fbe-8c0f-dd121924b6e0",
          "name": "merge-user-into-another-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/merge_into/accounts/destination_account_id/users/:destination_user_id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "destination_user_id",
                  "value": "destination_user_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Merge user into another user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b989614f-99ab-47a4-b6b0-829c666f27b7"
            }
          ]
        }
      ]
    }
  ]
}