{
  "info": {
    "name": "Instructure Canvas Calendar Events API Update a calendar event",
    "_postman_id": "3087635f-2d8a-4ae0-a2a1-d4e67ff1692a",
    "description": "Update a calendar event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calendar",
      "item": [
        {
          "id": "d2c445a9-0049-41a4-b471-12a2576a9c5a",
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
              "id": "98a70a76-8a85-4939-ba3a-f1520ffb0584"
            }
          ]
        },
        {
          "id": "a09390cd-68b4-45fd-b2c4-2012ffd186f4",
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
              "id": "7ae7d280-0b10-4a8f-b2f3-b92b395aec78"
            }
          ]
        },
        {
          "id": "4a118c5d-1b99-4749-8fd1-c7ec4eb7b1dc",
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
              "id": "6e853cfc-f94c-4136-8923-ff0c60f774c5"
            }
          ]
        },
        {
          "id": "da6a404c-0f84-4ca1-b99f-b0329cf9f2bd",
          "name": "update-a-calendar-event",
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
                  "key": "calendar_event[child_event_data][X][context_code]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[child_event_data][X][end_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[child_event_data][X][start_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[context_code]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[end_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[location_address]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[location_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[start_at]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[time_zone_edited]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "calendar_event[title]",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a calendar event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bdf3d97-b1b9-4632-beb2-9b81f2577752"
            }
          ]
        },
        {
          "id": "611f75f9-fe73-484b-8aa0-767ab9df24bd",
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
              "id": "6aa32cf9-786c-4356-ae99-37647fc7f227"
            }
          ]
        }
      ]
    }
  ]
}