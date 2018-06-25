{
  "info": {
    "name": "Instructure Canvas Groups API Get a single group category",
    "_postman_id": "eb428810-1fc8-4318-b2a3-5d77e43c356e",
    "description": "Get a single group category.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Group",
      "item": [
        {
          "id": "826f2550-0153-42a4-8174-be69806ee95f",
          "name": "get-a-single-group-category",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "group_categories/:group_category_id"
              ],
              "variable": [
                {
                  "id": "group_category_id",
                  "value": "group_category_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single group category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e71c895-70db-43c9-86f2-9bf6767a3640"
            }
          ]
        },
        {
          "id": "66074d3f-c954-4476-9263-421087509ff8",
          "name": "delete-a-group-category",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "group_categories/:group_category_id"
              ],
              "variable": [
                {
                  "id": "group_category_id",
                  "value": "group_category_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a group category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f93ff276-102b-422b-943e-d99e7a6b3048"
            }
          ]
        }
      ]
    }
  ]
}