{
  "info": {
    "name": "Instructure Canvas Sections API De-cross-list a Section",
    "_postman_id": "a5ce20c3-df0a-43df-a040-d3e1ec8caa93",
    "description": "De-cross-list a section.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Sections",
      "item": [
        {
          "id": "06d185a0-791f-4e65-b70e-95f894a21cd4",
          "name": "decrosslist-a-section",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "sections/:id/crosslist"
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
            "description": "De-cross-list a section."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9a83d94-c212-407d-bff2-c780c89a08a3"
            }
          ]
        }
      ]
    }
  ]
}