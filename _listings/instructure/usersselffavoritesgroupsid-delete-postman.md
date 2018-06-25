{
  "info": {
    "name": "Instructure Canvas Users API Remove group from favorites",
    "_postman_id": "88ffe6e5-bc1a-4016-93f0-2d607a08fefc",
    "description": "Remove group from favorites.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "4243907b-2c33-45d2-95cb-850b1ca80a5b",
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
              "id": "46d45759-2c87-4ccd-bfe0-0cacaf51cf03"
            }
          ]
        },
        {
          "id": "c4ed78bf-6c20-4b27-ad7f-6934f7f063c6",
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
              "id": "cbe89a7d-2d2a-40ae-b00c-893fcc35563a"
            }
          ]
        },
        {
          "id": "60ca6224-6c5e-4ee1-b438-3db7a018049a",
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
              "id": "01902d5a-a91e-4821-8db4-f2f8beae13e8"
            }
          ]
        },
        {
          "id": "d80ffa76-1a85-4c98-8319-03b4a8496dd6",
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
              "id": "8a2c72df-193d-48f9-aa4c-baf8f571227c"
            }
          ]
        },
        {
          "id": "07450621-582f-42df-90f5-494dbf2233e9",
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
              "id": "cc77f935-513f-49eb-b8f2-230dcc09ef79"
            }
          ]
        },
        {
          "id": "56d67575-388a-4b9c-9cc7-a1151f5831bf",
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
              "id": "15719603-f938-4980-839b-b334bfdf9928"
            }
          ]
        },
        {
          "id": "673241e8-f6dc-4785-a2ac-d6f30260a353",
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
              "id": "af80b4c8-c5f2-4b94-afb5-b6d5729116bc"
            }
          ]
        }
      ]
    }
  ]
}