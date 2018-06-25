{
  "info": {
    "name": "Instructure Canvas Groups API List content exports",
    "_postman_id": "ed609091-981f-4163-a04d-b242eed9003a",
    "description": "List content exports.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "d5ba0741-98e4-4aa3-9724-f1f95f784576",
          "name": "list-content-exports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports"
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
            "description": "List content exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95c6b580-c90e-40c0-8dbc-7f964a4556ad"
            }
          ]
        }
      ]
    }
  ]
}