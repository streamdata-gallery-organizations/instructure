{
  "info": {
    "name": "Instructure Canvas Sections API Get section information",
    "_postman_id": "f6d4f167-0143-48b7-b289-895926fa28b9",
    "description": "Get section information.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sections",
      "item": [
        {
          "id": "07767899-840e-495c-9808-acf28882038d",
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
              "id": "2a79791e-a1c0-4199-9d3d-8235c24322cb"
            }
          ]
        },
        {
          "id": "2ba82881-c3c2-4a1a-ab5b-5775084ad7ca",
          "name": "get-section-information",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get section information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b14b888-0d1a-4e16-8bb2-8578c63f54b7"
            }
          ]
        },
        {
          "id": "ef2ce667-87d6-4eca-85ee-22f4dd21028f",
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
              "id": "063fd41f-d3f9-4a02-819e-588f1b9751ab"
            }
          ]
        }
      ]
    }
  ]
}