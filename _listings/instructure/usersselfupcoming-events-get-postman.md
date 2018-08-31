{
  "info": {
    "name": "Instructure Canvas Users API List upcoming assignments, calendar events",
    "_postman_id": "0ddeaee7-ce46-46ed-9879-0c413f36349a",
    "description": "List upcoming assignments, calendar events.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "94a1b812-cd82-4202-b211-a9df57ee7af3",
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
              "id": "894f7a15-9d5f-4956-a92f-bfecdd4372d6"
            }
          ]
        }
      ]
    }
  ]
}