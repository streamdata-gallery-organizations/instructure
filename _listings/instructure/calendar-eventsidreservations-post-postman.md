{
  "info": {
    "name": "Instructure Canvas Calendar Events API Reserve a time slot",
    "_postman_id": "5f716963-e229-4a3f-aeaf-772ab2bca715",
    "description": "Reserve a time slot.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Calendar",
      "item": [
        {
          "id": "5912fea9-638b-4571-8cea-7a6b504dc8b2",
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
              "id": "f0fc7d35-d056-46b5-a392-165bccd1b0ec"
            }
          ]
        },
        {
          "id": "fea7818e-e0be-459d-a28c-0a03fd8c9817",
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
              "id": "d0c09584-7df1-4599-b3c1-3c719c906b47"
            }
          ]
        },
        {
          "id": "dcab4451-6fc3-49d0-976b-ba2fc8346191",
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
              "id": "47c3bcc5-8236-42c4-8b35-6d40457aeaf5"
            }
          ]
        },
        {
          "id": "be1adb6c-d665-43df-a891-44b9dc20ee80",
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
              "id": "3fec2c75-e972-4634-9fc5-6e341c890561"
            }
          ]
        },
        {
          "id": "da4b2ac3-1ff1-4b0c-828f-4effaf7b7c2f",
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
              "id": "7a1cf720-d282-4234-b4ff-da484262daa5"
            }
          ]
        },
        {
          "id": "df1a914f-7d30-497b-9e60-306a1aa75bbc",
          "name": "reserve-a-time-slot",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "calendar_events/:id/reservations"
              ],
              "query": [
                {
                  "key": "cancel_existing",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "comments",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "participant_id",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reserve a time slot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c92d18c4-9539-4c1b-9f5e-03223b421940"
            }
          ]
        }
      ]
    }
  ]
}