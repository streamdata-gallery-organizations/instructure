{
  "info": {
    "name": "Instructure Canvas Users API Store custom data",
    "_postman_id": "a5406354-32c0-49a2-ad8b-00571a837124",
    "description": "Store custom data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "5be40d6c-5b5f-4954-9154-d168c1757b14",
          "name": "load-custom-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/custom_data(/*scope)"
              ],
              "query": [
                {
                  "key": "ns",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Load custom data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cf670127-2995-459b-9315-039376ba70fc"
            }
          ]
        },
        {
          "id": "940ee89c-bf07-4922-82fb-fe0593568605",
          "name": "store-custom-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/custom_data(/*scope)"
              ],
              "query": [
                {
                  "key": "data",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ns",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Store custom data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11c27089-0746-43aa-8514-3f2816b70889"
            }
          ]
        },
        {
          "id": "d658bf77-52bc-4763-aca0-07b327dd43e7",
          "name": "delete-custom-data",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/custom_data(/*scope)"
              ],
              "query": [
                {
                  "key": "ns",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete custom data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "21a67b32-8175-4cf9-a9b7-a27015b4712f"
            }
          ]
        }
      ]
    }
  ]
}