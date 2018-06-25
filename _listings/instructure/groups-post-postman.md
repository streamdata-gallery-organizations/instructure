{
  "info": {
    "name": "Instructure Canvas Groups API Create a group",
    "_postman_id": "af846428-f8ee-4a0b-a3bd-87043970e5ec",
    "description": "Create a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "7fb2d9d6-efa8-4c23-bd97-2b5dc3989275",
          "name": "create-a-group",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/groups?description=%7B%7D&is_public=%7B%7D&join_level=%7B%7D&name=%7B%7D&storage_quota_mb=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "41cbb546-e2e6-4811-95c4-266104d732f6"
            }
          ]
        }
      ]
    }
  ]
}