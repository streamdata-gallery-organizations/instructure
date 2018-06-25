{
  "info": {
    "name": "Instructure Canvas Users API List your groups",
    "_postman_id": "ac76191f-b196-4305-87cc-ae0f20ef2ab3",
    "description": "List your groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "94d706f1-70a2-425f-ad24-3ebbe95c0b79",
          "name": "list-favorite-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/groups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List favorite groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43f8398d-fee4-4e71-97af-fe2cf86a3d74"
            }
          ]
        },
        {
          "id": "eb5a8a67-a49c-43b5-84b0-7f6883f12537",
          "name": "reset-group-favorites",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/groups",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Reset group favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "adc5e711-b2ea-4341-b588-7f7d88f67efa"
            }
          ]
        },
        {
          "id": "702c1234-9743-4ccd-aaef-74da808cf1db",
          "name": "add-group-to-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add group to favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfb679a1-f24a-4f4d-96f7-f56a1b3e953f"
            }
          ]
        },
        {
          "id": "3e3cfe22-f1a0-449a-bb74-dadb816cb0ee",
          "name": "remove-group-from-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove group from favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd910a22-1e67-4265-a599-785379c6949f"
            }
          ]
        },
        {
          "id": "acbcd4a2-b068-448f-a835-97f4601df958",
          "name": "list-your-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/groups?context_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List your groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ea8e77a-f505-4d89-80e0-26966dc6c940"
            }
          ]
        }
      ]
    }
  ]
}