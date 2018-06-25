{
  "info": {
    "name": "Instructure Canvas Groups API Create a group",
    "_postman_id": "e60c70ef-cbd4-4d48-915f-788243de9556",
    "description": "Create a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Group",
      "item": [
        {
          "id": "3f92d0cf-d135-42de-9fdc-2724b7d123b3",
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
              "id": "92056899-0a49-475c-944c-1da5b83045a6"
            }
          ]
        },
        {
          "id": "531cbc01-13b3-4247-a242-5b0bd7f14b3d",
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
              "id": "22a93e31-cf4e-4eba-b351-9bf9ca8ea9f6"
            }
          ]
        },
        {
          "id": "b869c0ae-7b3d-4ca4-a1cb-d523af25f64c",
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
              "id": "84822fa2-d97e-47b3-b0ea-5099bfb482ed"
            }
          ]
        },
        {
          "id": "325f6187-c75f-4630-85ed-c2f0e53f5c93",
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
              "id": "e8cb5716-e8b0-47bb-934e-762fe6890957"
            }
          ]
        },
        {
          "id": "fa9c1fb0-bfb9-4f51-ae7a-1ac0722e01ac",
          "name": "list-groups-in-group-category",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "group_categories/:group_category_id/groups"
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
            "description": "List groups in group category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b09a04fc-e227-406c-8d26-e0e79d588884"
            }
          ]
        },
        {
          "id": "ef06c723-37f7-42fc-a10c-7e5b6adeb2f3",
          "name": "create-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "group_categories/:group_category_id/groups"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_public",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "join_level",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "storage_quota_mb",
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
            "description": "Create a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a46651cf-9960-44d4-a467-ddb2a1c6b3a7"
            }
          ]
        }
      ]
    }
  ]
}