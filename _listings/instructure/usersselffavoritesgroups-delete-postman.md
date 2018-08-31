{
  "info": {
    "name": "Instructure Canvas Users API Reset group favorites",
    "_postman_id": "e3f0ef4e-277b-4366-a9b3-bdad5ad02e13",
    "description": "Reset group favorites.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "64ca85e9-d0ed-40e1-bf1a-f792f10b0413",
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
              "id": "eb3fab4f-f913-4101-b826-4fd9a5b5f640"
            }
          ]
        },
        {
          "id": "b7e4114d-bef9-4124-877b-51461574ace3",
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
              "id": "b65f5af6-4173-4e90-bc0a-36534f093294"
            }
          ]
        },
        {
          "id": "722d1eac-333e-4582-8661-da27ab62d626",
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
              "id": "3c7cba99-3f80-4e1f-a39b-7b43c76c6f73"
            }
          ]
        },
        {
          "id": "f754c064-d3c5-45c4-b74c-36859fe887ad",
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
              "id": "1a74f7a1-ada2-4ac1-b61f-101d29dc4832"
            }
          ]
        },
        {
          "id": "81777a54-8384-4eb5-af8d-8f4d0ad19696",
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
              "id": "ce1a4498-17f2-46fa-a25c-71249f292513"
            }
          ]
        }
      ]
    }
  ]
}