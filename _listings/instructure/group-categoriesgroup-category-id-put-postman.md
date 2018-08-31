{
  "info": {
    "name": "Instructure Canvas Groups API Update a Group Category",
    "_postman_id": "68adefb9-38ce-4077-bb34-3eb3292846d1",
    "description": "Update a group category.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Group",
      "item": [
        {
          "id": "35dbbca4-38f9-4f18-88e5-88fd32afc429",
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
              "id": "481af57f-86b6-4b1e-bf6a-f5843288fc2a"
            }
          ]
        },
        {
          "id": "cf11330d-caea-4192-8c29-376d428d4125",
          "name": "update-a-group-category",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "group_categories/:group_category_id"
              ],
              "query": [
                {
                  "key": "auto_leader",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "create_group_count",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "self_signup",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "split_group_count",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_category_id",
                  "value": "group_category_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a group category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cc443b2-6b38-439a-81c8-51baead6e804"
            }
          ]
        },
        {
          "id": "011101a7-d17b-462f-96f4-2781df5239cf",
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
              "id": "903aed6b-9e47-46ec-9cb8-c1543df7f1d6"
            }
          ]
        }
      ]
    }
  ]
}