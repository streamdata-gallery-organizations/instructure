{
  "info": {
    "name": "Instructure Canvas Utility APIs Create Error Report",
    "_postman_id": "5694d856-227a-4304-a0ad-ba001c5a3c80",
    "description": "Create error report.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Error",
      "item": [
        {
          "id": "09c97cfd-d05b-474b-926a-9db13fc821e9",
          "name": "create-error-report",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/error_reports?error[comments]=%7B%7D&error[email]=%7B%7D&error[http_env]=%7B%7D&error[subject]=%7B%7D&error[url]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create error report."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37bf55c4-5211-42eb-bbef-db79ade31b19"
            }
          ]
        }
      ]
    }
  ]
}