{
  "info": {
    "name": "Instructure Canvas Sections API Delete a section",
    "_postman_id": "71ba75a2-4d84-43fb-9dd5-176042e126b5",
    "description": "Delete a section.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sections",
      "item": [
        {
          "id": "ac0d098d-8cf8-402e-ab2c-427fb902b1cf",
          "name": "redirect-to-the-assignment-override-for-a-section",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "sections/:course_section_id/assignments/assignment_id/override"
              ],
              "variable": [
                {
                  "id": "course_section_id",
                  "value": "course_section_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Redirect to the assignment override for a section."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "102d14d9-aba1-4d86-9bab-569343d7b2ea"
            }
          ]
        },
        {
          "id": "b15b8174-0d2c-478b-a47b-e055f4d30b45",
          "name": "delete-a-section",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "sections/:id"
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
            "description": "Delete a section."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9aaf9c34-cce8-48f6-ab5d-2822f122a93d"
            }
          ]
        }
      ]
    }
  ]
}