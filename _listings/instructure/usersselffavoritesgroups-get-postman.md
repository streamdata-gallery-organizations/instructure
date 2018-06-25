{
  "info": {
    "name": "Instructure Canvas Users API List favorite groups",
    "_postman_id": "07261ef4-6297-4893-a677-5c6ec839e174",
    "description": "List favorite groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "dee2c535-6518-4fee-9db3-e1e579d18f3e",
          "name": "list-favorite-courses",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/courses",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List favorite courses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bed0138c-d133-47f3-bcb6-8e50f575f2d7"
            }
          ]
        },
        {
          "id": "3180c1dd-f14e-4106-949d-9964337ef2a5",
          "name": "reset-course-favorites",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/courses",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Reset course favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b3bcb74-a867-4c6f-a542-825a0a311e9c"
            }
          ]
        },
        {
          "id": "269e813c-300e-4a68-918a-a63e39d21273",
          "name": "add-course-to-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/courses/:id"
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
            "description": "Add course to favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25a713ce-f0d6-4c33-b98b-e144c8730522"
            }
          ]
        },
        {
          "id": "39481772-5041-4b89-9124-360227530c87",
          "name": "remove-course-from-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/courses/:id"
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
            "description": "Remove course from favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b856fd26-c419-4925-8330-1c3b6da91fdc"
            }
          ]
        },
        {
          "id": "b0761123-db7a-49d4-868d-51ce62435564",
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
              "id": "d6b38142-a0e7-46e5-8def-92015fbdd3dd"
            }
          ]
        },
        {
          "id": "1ad3e201-6c88-48ef-9fc2-fb2f05ef089d",
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
              "id": "cfae5d83-3e1d-4ece-b0c4-10cc7cded37c"
            }
          ]
        }
      ]
    }
  ]
}