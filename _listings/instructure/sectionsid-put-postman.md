{
  "info": {
    "name": "Instructure Canvas Sections API Edit a section",
    "_postman_id": "970961b0-dd6b-4b31-a9ab-e63ac1a621ef",
    "description": "Edit a section.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sections",
      "item": [
        {
          "id": "1e432dd6-de99-46a7-beb3-e6f80e5d4f9d",
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
              "id": "f84680dd-2322-47ca-ad1c-09a9d74a0bb3"
            }
          ]
        },
        {
          "id": "9a92a1cd-2151-4443-b739-978bbc4b4f05",
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
              "id": "b82e2cc2-7506-4eaa-b1c1-abe6c531f5ae"
            }
          ]
        },
        {
          "id": "431d9612-b975-4fb8-936f-54a9254e3e4b",
          "name": "edit-a-section",
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
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a section."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b2c2069-5a14-499e-9f14-ec06f3683207"
            }
          ]
        },
        {
          "id": "cc04e359-e5b2-47d1-9f4b-a530d13d30c2",
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
              "id": "9efbb98b-0d6e-4398-9833-a8882056ecab"
            }
          ]
        }
      ]
    }
  ]
}