{
  "info": {
    "name": "Instructure Canvas Users API Delete custom data",
    "_postman_id": "59bb9af6-fa9b-43fd-b7a5-a8e70bbd54f1",
    "description": "Delete custom data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "a4e098db-01cf-4c57-96b5-3f90d23e96b8",
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
              "id": "2fdb6ab3-6cc1-4e41-921c-c4fcff62b733"
            }
          ]
        }
      ]
    }
  ]
}