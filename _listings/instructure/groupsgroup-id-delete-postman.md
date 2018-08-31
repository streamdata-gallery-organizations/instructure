{
  "info": {
    "name": "Instructure Canvas Groups API Delete a group",
    "_postman_id": "0975aac2-88b0-4418-93b1-796991b72858",
    "description": "Delete a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "fbb2a3d6-5f1e-4d86-bdd6-a58967713252",
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
              "id": "55c30bbe-77af-44d4-aef6-1fd5d9d54387"
            }
          ]
        },
        {
          "id": "7d785b99-d780-45f6-8de1-fd643b44075f",
          "name": "delete-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89f3c9a6-fa3f-49ac-acb0-02f1f973bb49"
            }
          ]
        }
      ]
    }
  ]
}