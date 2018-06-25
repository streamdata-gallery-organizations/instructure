{
  "info": {
    "name": "Instructure Canvas Groups API List groups in group category",
    "_postman_id": "dd593c22-6155-44d3-b997-30f2ac82b6c3",
    "description": "List groups in group category.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Group",
      "item": [
        {
          "id": "3b9189b4-83d8-408f-bde8-0f3dd29f2add",
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
              "id": "faed0218-655a-4c7e-ba64-037489d83c1a"
            }
          ]
        },
        {
          "id": "c8d55202-12d3-4d50-bade-1eebd5c2be27",
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
              "id": "8df6be15-7afa-4430-bbf1-4662d3adf06f"
            }
          ]
        },
        {
          "id": "10e6653c-243a-419a-ba7c-db56935bc9aa",
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
              "id": "f8beae76-33be-40b5-b9ba-906a75065ddb"
            }
          ]
        },
        {
          "id": "76b08a3e-902a-4c27-a1ba-3bc4ecb7622b",
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
              "id": "29db16dd-1278-40a6-a4f7-90257b41da6c"
            }
          ]
        },
        {
          "id": "4d275d3c-56db-4935-9a96-2a411c4c173a",
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
              "id": "b8af50d6-5c54-47e1-a8f8-5215d9f9a555"
            }
          ]
        }
      ]
    }
  ]
}