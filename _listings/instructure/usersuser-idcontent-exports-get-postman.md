{
  "info": {
    "name": "Instructure Canvas Users API List content exports",
    "_postman_id": "75b34d41-3037-466f-bea6-2ed6240d0509",
    "description": "List content exports.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "e4289984-ee3a-48bc-bd92-288bdab85518",
          "name": "list-content-exports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_exports"
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
            "description": "List content exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cbd8099-d5e7-4648-976e-9cc89e325247"
            }
          ]
        }
      ]
    }
  ]
}