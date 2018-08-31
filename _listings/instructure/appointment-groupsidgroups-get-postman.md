{
  "info": {
    "name": "Instructure Canvas Appointment Groups API List student group participants",
    "_postman_id": "e44c676d-e0a9-447f-8817-77f607571109",
    "description": "List student group participants.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Appointment",
      "item": [
        {
          "id": "213df421-64cf-496f-ad78-30efd7f62757",
          "name": "list-appointment-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/appointment_groups?context_codes=%5B%7B%7D%5D&include=%5B%7B%7D%5D&include_past_appointments=%7B%7D&scope=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List appointment groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "154ebfdc-af36-450a-b08c-8b33b276cdc3"
            }
          ]
        },
        {
          "id": "97b81782-01a6-43bf-8fa0-fb6aeb7f78fd",
          "name": "create-an-appointment-group",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/appointment_groups?appointment_group[context_codes=%5B%7B%7D%5D&appointment_group[description]=%7B%7D&appointment_group[location_address]=%7B%7D&appointment_group[location_name]=%7B%7D&appointment_group[max_appointments_per_participant]=%7B%7D&appointment_group[min_appointments_per_participant]=%7B%7D&appointment_group[new_appointments][X=%5B%7B%7D%5D&appointment_group[participants_per_appointment]=%7B%7D&appointment_group[participant_visibility]=%7B%7D&appointment_group[publish]=%7B%7D&appointment_group[sub_context_codes=%5B%7B%7D%5D&appointment_group[title]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65c5d01e-8aad-4709-91c4-773d743b9e7a"
            }
          ]
        },
        {
          "id": "b4cafe39-0ab8-4f11-a052-db694453f2eb",
          "name": "get-a-single-appointment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e46aded-3e69-4cb2-af66-9883d0efd864"
            }
          ]
        },
        {
          "id": "0dee8b35-d4ee-49b8-bf84-74146d3006b0",
          "name": "update-an-appointment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id"
              ],
              "query": [
                {
                  "key": "appointment_group[context_codes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[description]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[location_address]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[location_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[max_appointments_per_participant]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[min_appointments_per_participant]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[new_appointments][X",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[participants_per_appointment]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[participant_visibility]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[publish]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[sub_context_codes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "appointment_group[title]",
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
            "description": "Update an appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05582548-4bb4-43b8-abe1-d4a9023fcf0e"
            }
          ]
        },
        {
          "id": "c53ea48d-1498-40f7-8624-f529b5d70071",
          "name": "delete-an-appointment-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id"
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
            "description": "Delete an appointment group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a7c2a71-06c5-41fb-a4ce-95711ba8db81"
            }
          ]
        },
        {
          "id": "848bf98a-62e0-4571-b421-db87293c65e1",
          "name": "list-student-group-participants",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "appointment_groups/:id/groups"
              ],
              "query": [
                {
                  "key": "registration_status",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List student group participants."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd863a5d-455e-40e6-b510-a43d6c314919"
            }
          ]
        }
      ]
    }
  ]
}