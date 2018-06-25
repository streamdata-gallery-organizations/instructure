{
  "info": {
    "name": "Instructure Canvas Calendar Events API Create a calendar event",
    "_postman_id": "9646fb19-5322-43f1-b16b-afd850710d46",
    "description": "Create a calendar event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calendar",
      "item": [
        {
          "id": "d257c125-0f0c-438d-8d98-eb8fe091b388",
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
              "id": "eb49f06f-f2b6-420c-935c-a58266998dd0"
            }
          ]
        },
        {
          "id": "53d0b625-97da-446e-af1a-8277900ac214",
          "name": "create-a-calendar-event",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/calendar_events?calendar_event[child_event_data][X][context_code]=%7B%7D&calendar_event[child_event_data][X][end_at]=%7B%7D&calendar_event[child_event_data][X][start_at]=%7B%7D&calendar_event[context_code]=%7B%7D&calendar_event[description]=%7B%7D&calendar_event[duplicate][append_iterator]=%7B%7D&calendar_event[duplicate][count]=%7B%7D&calendar_event[duplicate][frequency]=%7B%7D&calendar_event[duplicate][interval]=%7B%7D&calendar_event[end_at]=%7B%7D&calendar_event[location_address]=%7B%7D&calendar_event[location_name]=%7B%7D&calendar_event[start_at]=%7B%7D&calendar_event[time_zone_edited]=%7B%7D&calendar_event[title]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a calendar event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10284c74-68ba-4b78-b8c1-aa7a48276c27"
            }
          ]
        }
      ]
    }
  ]
}