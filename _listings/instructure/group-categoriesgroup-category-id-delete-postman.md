{
  "info": {
    "name": "Instructure Canvas Groups API Delete a Group Category",
    "_postman_id": "b21bc12d-09fd-4d7d-8fd0-0553e9bcf50d",
    "description": "Delete a group category.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Group",
      "item": [
        {
          "id": "d554b62a-77a6-4fb7-b1dc-7128489cf6a7",
          "name": "delete-a-group-category",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "group_categories/:group_category_id"
              ],
              "variable": [
                {
                  "id": "group_category_id",
                  "value": "group_category_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a group category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d33ebc1-2c0f-4340-a514-0c86b148e599"
            }
          ]
        }
      ]
    }
  ]
}