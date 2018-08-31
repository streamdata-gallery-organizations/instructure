{
  "info": {
    "name": "Instructure Canvas Utility APIs List members of a collaboration.",
    "_postman_id": "d61aa567-f8e6-4f89-a76d-ca9b6599d9ce",
    "description": "List members of a collaboration..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Collaborations",
      "item": [
        {
          "id": "9dc25d0d-9392-4428-9544-b8ce9e8ffaf6",
          "name": "list-members-of-a-collaboration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "collaborations/:id/members"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List members of a collaboration.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9619036d-7efc-4c7f-9703-7084816cff24"
            }
          ]
        }
      ]
    }
  ]
}