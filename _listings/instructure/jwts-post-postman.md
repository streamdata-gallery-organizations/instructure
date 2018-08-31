{
  "info": {
    "name": "Instructure Canvas Utility APIs Create JWT",
    "_postman_id": "f3a68808-5743-44ff-a26e-b8a3706b0ad3",
    "description": "Create jwt.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Api",
      "item": [
        {
          "id": "80d06604-d324-45ad-8152-5e1ddb953926",
          "name": "retrieve-assignments-enabled-for-grade-export-to-sis",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "api/sis/accounts/:account_id/assignments"
              ],
              "query": [
                {
                  "key": "course_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ends_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starts_before",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve assignments enabled for grade export to sis."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "762da172-6bfe-48be-b16b-87b0f6549fab"
            }
          ]
        },
        {
          "id": "c4253cf8-f46a-46c1-b5d8-eb4156167b36",
          "name": "retrieve-assignments-enabled-for-grade-export-to-sis1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "api/sis/courses/:course_id/assignments"
              ],
              "query": [
                {
                  "key": "account_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "ends_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "starts_before",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve assignments enabled for grade export to sis."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "baffd3eb-b5c3-4863-8a17-4f9d052ed89d"
            }
          ]
        }
      ]
    },
    {
      "name": "Collaborations",
      "item": [
        {
          "id": "970065af-822c-4ffb-8e60-158503eff6b3",
          "name": "list-members-of-a-collaboration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "collaborations/:id/members"
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
            "description": "List members of a collaboration.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfacf804-cf93-4c41-adb1-1c24f551d064"
            }
          ]
        }
      ]
    },
    {
      "name": "Comm",
      "item": [
        {
          "id": "4268c3e9-c55a-4778-9980-4ab65321d7bd",
          "name": "list-of-commmessages-for-a-user",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/comm_messages?end_time=%7B%7D&start_time=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of commmessages for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cd4414a-4a07-4f4b-9b52-ffc084f280f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Course",
      "item": [
        {
          "id": "677d9d40-7acc-4dcb-a32f-48abab236c77",
          "name": "list-accounts-for-course-admins",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/course_accounts",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List accounts for course admins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb922aaf-cb91-41c2-a4bc-d2e03f616654"
            }
          ]
        }
      ]
    },
    {
      "name": "Error",
      "item": [
        {
          "id": "5e521a6c-846d-4292-bf26-84c5cb8c6f69",
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
              "id": "50e6f927-58b2-48e9-801a-7c91aea8e7cf"
            }
          ]
        }
      ]
    },
    {
      "name": "Jwts",
      "item": [
        {
          "id": "dc8749c5-1a97-4717-a42f-98317e64a823",
          "name": "create-jwt",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/jwts",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create jwt."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "558659ca-76f9-467b-9a4b-efe811c71cbb"
            }
          ]
        }
      ]
    }
  ]
}