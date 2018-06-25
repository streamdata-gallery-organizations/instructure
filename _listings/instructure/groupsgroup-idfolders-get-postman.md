{
  "info": {
    "name": "Instructure Canvas Groups API List all folders",
    "_postman_id": "23cfeec8-e683-40a7-bea4-b118615e0415",
    "description": "List all folders.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "e198d2d7-2ce4-43b7-b9b3-6163a98c8390",
          "name": "list-all-folders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/folders"
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
            "description": "List all folders."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ef3bc7f-9b9c-4338-94d4-5f99c628976d"
            }
          ]
        }
      ]
    }
  ]
}