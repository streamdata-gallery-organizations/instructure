{
  "info": {
    "name": "Instructure Canvas Appointment Groups API List appointment groups",
    "_postman_id": "7ecd58cc-6ad8-4656-8baf-3067456ddc8d",
    "description": "List appointment groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Appointment",
      "item": [
        {
          "id": "1471bf07-2a00-4bf2-add0-caa5a8779c1f",
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
              "id": "0c44632e-dda8-4898-93b3-51b6073c2ea8"
            }
          ]
        }
      ]
    }
  ]
}