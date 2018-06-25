{
  "info": {
    "name": "Instructure Canvas Groups API Resolve path",
    "_postman_id": "1a5cb679-51a8-4baf-bd87-5b334bee0a88",
    "description": "Resolve path.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "cea27698-c819-4d4b-9022-d334384f9959",
          "name": "list-all-folders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/folders"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all folders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a37e4f0-dfa3-456e-bead-8da22e6690c6"
            }
          ]
        },
        {
          "id": "0aebbd7c-82e5-4a29-b35e-cd2b4fc7bbd1",
          "name": "create-folder",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/folders"
              ],
              "query": [
                {
                  "key": "hidden",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "locked",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "parent_folder_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "parent_folder_path",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "unlock_at",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create folder."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c05de65f-ef24-423d-816c-8c238a334d83"
            }
          ]
        },
        {
          "id": "59c90601-f2a1-4a3f-80c9-376f363bae68",
          "name": "resolve-path",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/folders/by_path"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resolve path."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5627382b-ebc0-4d3a-9c23-2c8fddc0011c"
            }
          ]
        },
        {
          "id": "c0852524-cac1-4c7d-84cb-4f52416dd48e",
          "name": "resolve-path1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/folders/by_path/*full_path"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resolve path."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faa0bddf-2146-4a16-adc8-828cbdaeaf49"
            }
          ]
        }
      ]
    }
  ]
}