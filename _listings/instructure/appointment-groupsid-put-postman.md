{
  "info": {
    "name": "Instructure Canvas Appointment Groups API Update an appointment group",
    "_postman_id": "4b2e8576-5ff6-4e5e-a70b-f1042fae48de",
    "description": "Update an appointment group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Appointment",
      "item": [
        {
          "id": "11a0c3f0-dec9-4bff-ae96-29bbbf377820",
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
              "id": "24866131-6ada-4108-b80a-dc318ab2685b"
            }
          ]
        },
        {
          "id": "77b83b24-0cb7-4146-bba6-c16f41dd80ae",
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
              "id": "eb7bede6-749c-4604-ab3d-3322d2e02211"
            }
          ]
        },
        {
          "id": "7c635bd9-1c94-4164-968a-2bacf27c0650",
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
              "id": "c040880b-af3b-43ba-b95f-e9b2ce232522"
            }
          ]
        },
        {
          "id": "b4030972-0d12-4d3a-800a-9836f8bd0df1",
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
              "id": "862e5747-03eb-4d75-958f-fdb0379153ac"
            }
          ]
        },
        {
          "id": "8002ae8e-881c-4082-aeb1-306e6423d6d1",
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
              "id": "b9d31a7a-2908-4f01-a1e5-497c065b0fa1"
            }
          ]
        }
      ]
    }
  ]
}