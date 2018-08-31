{
  "info": {
    "name": "Instructure Canvas Calendar Events API List calendar events",
    "_postman_id": "a32717ae-f85f-4326-a896-d29cfe99343e",
    "description": "List calendar events.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calendar",
      "item": [
        {
          "id": "ab016ee4-d982-4a77-b988-fc91789a1d16",
          "name": "list-calendar-events",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/calendar_events?all_events=%7B%7D&context_codes=%5B%7B%7D%5D&end_date=%7B%7D&excludes=%5B%7B%7D%5D&start_date=%7B%7D&type=%7B%7D&undated=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List calendar events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99826de0-b805-4bd7-852c-da7eefa29802"
            }
          ]
        }
      ]
    }
  ]
}