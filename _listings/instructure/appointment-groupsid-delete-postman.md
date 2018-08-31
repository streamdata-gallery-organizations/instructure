{
  "info": {
    "name": "Instructure Canvas Appointment Groups API Delete an appointment group",
    "_postman_id": "7be673f2-7b77-423a-a711-a258b1ce199d",
    "description": "Delete an appointment group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Appointment",
      "item": [
        {
          "id": "29db1f37-4f6a-4ce9-8619-99293ec41c6e",
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
              "id": "d0270f77-94ee-4985-a4ca-0d5b639a4a08"
            }
          ]
        },
        {
          "id": "0cb32330-aa33-463c-961a-9625bf5cd914",
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
              "id": "ce6b8e9e-7b66-4907-a90b-f383380ecf88"
            }
          ]
        },
        {
          "id": "262ccd6f-ef0b-40c7-aba8-65f3f747007b",
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
              "id": "46751d36-8f08-47e1-a711-2f4d6a3f99db"
            }
          ]
        }
      ]
    }
  ]
}