{
  "info": {
    "name": "Instructure Canvas Calendar Events API Get a single calendar event or assignment",
    "_postman_id": "8edde8ed-1653-4a68-bb4e-849e6a668d3a",
    "description": "Get a single calendar event or assignment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calendar",
      "item": [
        {
          "id": "5f17be34-d57c-4fad-9ad2-5898e4334428",
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
              "id": "93a46921-821b-4f0b-8024-70821343db31"
            }
          ]
        },
        {
          "id": "b32ab075-d900-45c4-aa4b-c76abcf74d9b",
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
              "id": "ad7bcd1f-5f57-43f9-b60f-3a97b756b39e"
            }
          ]
        },
        {
          "id": "83f9571d-9f77-475d-b6c8-e0a5c2aad9b0",
          "name": "get-a-single-calendar-event-or-assignment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "calendar_events/:id"
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
            "description": "Get a single calendar event or assignment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1694e255-36e1-43c0-b472-d18cb943bb2e"
            }
          ]
        },
        {
          "id": "68493779-bc07-473a-91da-77a4ff042261",
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
              "id": "71f7344e-e12b-4c61-906b-b053b4946ac2"
            }
          ]
        }
      ]
    }
  ]
}