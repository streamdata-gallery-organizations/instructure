{
  "info": {
    "name": "Instructure Canvas Groups API Assign unassigned members",
    "_postman_id": "32fbb5e9-36d0-446a-b6d3-b0d81d17afa4",
    "description": "Assign unassigned members.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Group",
      "item": [
        {
          "id": "698812a0-b035-40d5-a697-5c45de2718e0",
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
              "id": "7bf3c5e1-7449-4cdc-b042-7d41157f4386"
            }
          ]
        },
        {
          "id": "f4a97b8e-f402-4c87-86bc-22cd9227a405",
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
              "id": "99536715-5cd3-4f41-8482-e2d574c76d26"
            }
          ]
        },
        {
          "id": "a56eb5d1-2d86-4b22-b69c-8309ea76164c",
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
              "id": "38b4ef62-cfaa-4648-82f3-ab36b272902d"
            }
          ]
        },
        {
          "id": "fad219d1-9074-4ff2-9cb3-cf861ec551e4",
          "name": "assign-unassigned-members",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "group_categories/:group_category_id/assign_unassigned_members"
              ],
              "query": [
                {
                  "key": "sync",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Assign unassigned members."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad5f54f3-06b0-43b2-862b-75f6b2bacb51"
            }
          ]
        }
      ]
    }
  ]
}