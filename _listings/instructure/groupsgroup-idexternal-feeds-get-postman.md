{
  "info": {
    "name": "Instructure Canvas Groups API List external feeds",
    "_postman_id": "836ad18a-323d-4db4-b3c6-0f1160e855b6",
    "description": "List external feeds.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "50781520-fa74-4786-9922-6bbcdc80c7a7",
          "name": "list-external-feeds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/external_feeds"
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
            "description": "List external feeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee05d342-618e-46e6-88a6-64091538269a"
            }
          ]
        }
      ]
    }
  ]
}