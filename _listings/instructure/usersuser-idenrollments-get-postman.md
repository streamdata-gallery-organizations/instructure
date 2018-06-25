{
  "info": {
    "name": "Instructure Canvas Users API List enrollments",
    "_postman_id": "3f7e47e7-1db9-4bd7-a1b2-ca497e8b3bca",
    "description": "List enrollments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "63ea3e7f-8d63-4b11-9d1e-4fff2dee3d0d",
          "name": "list-enrollments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/enrollments"
              ],
              "query": [
                {
                  "key": "grading_period_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "role",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List enrollments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da3d99bc-eeb3-4993-8a82-aad3bbf3318d"
            }
          ]
        }
      ]
    }
  ]
}