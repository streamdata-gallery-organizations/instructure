{
  "info": {
    "name": "Instructure Canvas Users API List calendar events for a user",
    "_postman_id": "417c5520-0e57-4dcf-8cd4-b82a7419b244",
    "description": "List calendar events for a user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "33e5f7d0-1526-43b8-8d15-8145e6c31f75",
          "name": "list-upcoming-assignments-calendar-events",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/upcoming_events",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List upcoming assignments, calendar events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e748c4c-88bd-444c-9d45-7e85ffb8d7b2"
            }
          ]
        },
        {
          "id": "ea6bb752-5626-4c34-856a-fc33c965f9af",
          "name": "list-calendar-events-for-a-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/calendar_events"
              ],
              "query": [
                {
                  "key": "all_events",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "context_codes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "excludes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "undated",
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
            "description": "List calendar events for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1299b2d5-7a68-44ac-aad7-858a7eedb7cf"
            }
          ]
        }
      ]
    }
  ]
}