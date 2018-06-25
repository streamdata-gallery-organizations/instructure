{
  "info": {
    "name": "Instructure Canvas Users API Get a content migration",
    "_postman_id": "e9729fd7-6aae-47ce-98a2-54398c927464",
    "description": "Get a content migration.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "074797c1-7a76-4148-8515-6b55bbcaa905",
          "name": "list-content-exports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_exports"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ee9c053-e089-4dfd-b9d3-1131bd9587c3"
            }
          ]
        },
        {
          "id": "b71dfb9f-ef42-49e8-ac65-8311ccd90fb6",
          "name": "export-content",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_exports"
              ],
              "query": [
                {
                  "key": "export_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip_notifications",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Export content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02731ec2-0049-4e19-b4cd-12da6b24c024"
            }
          ]
        },
        {
          "id": "e6e3a9e8-b99b-4091-8f1c-461dda63c2e4",
          "name": "show-content-export",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_exports/id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show content export."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d744aa7-3799-41ce-9757-8c022a62be24"
            }
          ]
        },
        {
          "id": "c7b726ff-14a9-456c-ae85-849a9b705d7a",
          "name": "list-licenses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_licenses"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List licenses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcbe7adb-715c-4b0d-bc9e-d30748299f37"
            }
          ]
        },
        {
          "id": "ae4b94a0-867a-4edb-86b5-2a8094336c0b",
          "name": "list-content-migrations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content migrations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bb42872-94c9-430d-8331-52f6ee2eea87"
            }
          ]
        },
        {
          "id": "91789f56-5330-4b4b-ae93-6e439957258c",
          "name": "create-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations"
              ],
              "query": [
                {
                  "key": "date_shift_options[day_substitutions][X]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[remove_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[shift_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "migration_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[*]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[file_url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[folder_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[overwrite_quizzes]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[source_course_id]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2858013d-9310-4658-afbb-f99a9bf370f4"
            }
          ]
        },
        {
          "id": "3e18ea11-8425-41cf-83ce-a88b935c768d",
          "name": "list-migration-issues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations/content_migration_id/migration_issues"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List migration issues."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f61f80aa-1d94-4960-af87-2871148c3830"
            }
          ]
        },
        {
          "id": "4d6fc6e5-6337-42d9-af7c-aeb7a7c8b9ff",
          "name": "get-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
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
            "description": "Get a migration issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42d9abf6-8bf2-4c7f-8d62-94f2fc346ba3"
            }
          ]
        },
        {
          "id": "dd35c4da-16b0-4813-9b4d-175865ac32de",
          "name": "update-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "query": [
                {
                  "key": "workflow_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a migration issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90668d67-7658-4f88-81b7-05e7bacdf016"
            }
          ]
        },
        {
          "id": "0b272e08-7e1e-41b3-a745-326541996772",
          "name": "get-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations/id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1779aa39-5c13-4ef7-88f3-c9e277be4a79"
            }
          ]
        }
      ]
    }
  ]
}