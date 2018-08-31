{
  "info": {
    "name": "Instructure Canvas Groups API Redirect to the assignment override for a group",
    "_postman_id": "8b102c53-e40e-4334-9038-0fbd8067886a",
    "description": "Redirect to the assignment override for a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "fcc96ab2-d15a-4e57-b098-507f3d06ee03",
          "name": "redirect-to-the-assignment-override-for-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/assignments/assignment_id/override"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Redirect to the assignment override for a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ea2916e-1ae1-46ed-be2e-eefdb590284c"
            }
          ]
        }
      ]
    }
  ]
}