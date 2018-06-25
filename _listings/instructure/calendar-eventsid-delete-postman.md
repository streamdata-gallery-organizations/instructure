{
  "info": {
    "name": "Instructure Canvas Calendar Events API Delete a calendar event",
    "_postman_id": "a532bbf9-6b79-4ec3-b9c4-e04fa45d366c",
    "description": "Delete a calendar event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calendar",
      "item": [
        {
          "id": "3b193ba8-994d-4d31-93fa-eb4d5c9a46dd",
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
              "id": "470c96bb-e3d8-4a57-a19d-e7d0549ea7f3"
            }
          ]
        },
        {
          "id": "687922c0-2935-4e56-8987-367458ccabc4",
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
              "id": "b2405757-d7ce-4398-b66d-968c085cf11c"
            }
          ]
        },
        {
          "id": "15a23be8-e864-428f-8faf-317e05b6d509",
          "name": "delete-a-calendar-event",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "calendar_events/:id"
              ],
              "query": [
                {
                  "key": "cancel_reason",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a calendar event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28d93d0d-d4ea-47e7-bcbb-f95c7ef2df09"
            }
          ]
        }
      ]
    }
  ]
}