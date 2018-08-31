{
  "info": {
    "name": "Instructure Canvas Sections API Get all Peer Reviews",
    "_postman_id": "971eb3e0-94c0-47ec-9fbd-f9e374d4da9c",
    "description": "Get all peer reviews.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sections",
      "item": [
        {
          "id": "822808e7-f8cc-4a34-916c-3099584b687a",
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
              "id": "9428e440-b66f-4a38-a29d-aaaac4e14ba5"
            }
          ]
        },
        {
          "id": "9651459b-28e8-4316-9aeb-6894d7513243",
          "name": "get-all-peer-reviews",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "sections/:section_id/assignments/assignment_id/peer_reviews"
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
                  "id": "section_id",
                  "value": "section_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get all peer reviews."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1825efd6-5cc5-4a20-927d-073f1e27f849"
            }
          ]
        }
      ]
    }
  ]
}