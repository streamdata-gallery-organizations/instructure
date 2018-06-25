{
  "info": {
    "name": "Instructure Canvas Groups API Create page",
    "_postman_id": "5d178610-fab3-46d8-a7d7-6663c9b57777",
    "description": "Create page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Groups",
      "item": [
        {
          "id": "22d5430a-4686-41f0-b612-a3e4d4c958e0",
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
              "id": "9997c004-f961-4add-8d31-594674829cef"
            }
          ]
        },
        {
          "id": "d0b9347a-adf1-4c30-beaf-0a689b057635",
          "name": "get-a-single-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
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
            "description": "Get a single group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "006d7855-e4fc-4862-96a5-b25ccdeddf25"
            }
          ]
        },
        {
          "id": "94dac574-dc60-4ba9-9599-271da31b366e",
          "name": "edit-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id"
              ],
              "query": [
                {
                  "key": "avatar_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_public",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "join_level",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "members",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "storage_quota_mb",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2f305a0-2b05-4c0d-8e79-349e5b0ef165"
            }
          ]
        },
        {
          "id": "cf18404e-e0f5-4aac-9b8f-0cb83ed159e3",
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
              "id": "3601627c-7158-4825-9fdd-f9277f0f7e1b"
            }
          ]
        },
        {
          "id": "ebf95b60-43f8-48b8-a41a-199da1aea536",
          "name": "group-activity-stream",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/activity_stream"
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
            "description": "Group activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5974f6f3-4e56-4fd2-88e9-0ec968bb4651"
            }
          ]
        },
        {
          "id": "83136a0b-cb1d-4daf-a8f1-4b704a240a11",
          "name": "group-activity-stream-summary",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/activity_stream/summary"
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
            "description": "Group activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3ecec45-7a16-46ba-9d5a-5bb7d19b29a0"
            }
          ]
        },
        {
          "id": "aa2d5e4d-74bc-403c-8bdc-3a6d6101a67f",
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
              "id": "6a56f6c1-3a42-4a45-a31e-b77dbb29f6d0"
            }
          ]
        },
        {
          "id": "6639f231-7ee8-42f8-8a84-0c99793a9f0b",
          "name": "list-conferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/conferences"
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
            "description": "List conferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5502617e-615f-4673-9ad7-8847125e6b03"
            }
          ]
        },
        {
          "id": "5e80c3c4-b617-4e6b-af3d-ddbc7f39dcb0",
          "name": "list-content-exports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports"
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
            "description": "List content exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9dc5c603-01cd-462c-a6a9-77b65d0133b0"
            }
          ]
        },
        {
          "id": "c066e701-ea23-447a-81fd-2527b8a6c9f7",
          "name": "export-content",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports"
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
                  "id": "group_id",
                  "value": "group_id",
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
              "id": "2c39689e-3ea0-42a8-b0ac-330a837f7bd4"
            }
          ]
        },
        {
          "id": "753b573b-d240-4b1d-8552-aafc22a8a5fb",
          "name": "show-content-export",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_exports/id"
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
            "description": "Show content export."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "683f043c-7295-4288-8336-55e6aa501ba3"
            }
          ]
        },
        {
          "id": "541c34df-8b46-48a3-92a4-107f82f9079c",
          "name": "list-licenses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_licenses"
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
            "description": "List licenses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e7e912a-497e-421f-a18e-2dffc9301f3d"
            }
          ]
        },
        {
          "id": "d3f6151f-873e-45ca-a87a-ddc94212d658",
          "name": "list-content-migrations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations"
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
            "description": "List content migrations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01fbe1c9-774b-444b-8c91-9286fdba08fd"
            }
          ]
        },
        {
          "id": "77f69c10-2e33-48e4-9ae9-4bce275bf777",
          "name": "create-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations"
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
                  "id": "group_id",
                  "value": "group_id",
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
              "id": "546c6123-d2bc-4d7c-b8a9-056143f02ddb"
            }
          ]
        },
        {
          "id": "acc18845-eb3a-4b7e-95a7-85a42fa25045",
          "name": "list-migration-issues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues"
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
            "description": "List migration issues."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07eedebd-e4d1-4c2d-b55f-66108bde10d9"
            }
          ]
        },
        {
          "id": "608c7a4d-90de-49f7-92f1-0390cd534640",
          "name": "get-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
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
              "id": "f1108618-5203-4c0a-adf6-a797ae74b05f"
            }
          ]
        },
        {
          "id": "6c35fd96-254c-412e-82a4-3c2f8e5d4e6a",
          "name": "update-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/content_migration_id/migration_issues/:id"
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
                  "id": "group_id",
                  "value": "group_id",
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
              "id": "f3da01f7-e6b7-43d7-967d-3e707a89c5e7"
            }
          ]
        },
        {
          "id": "e8955e66-eb54-420c-8c54-ea5329ae48db",
          "name": "get-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/id"
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
            "description": "Get a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3cfe16c-fd2d-46c6-8532-4a25fc762d28"
            }
          ]
        },
        {
          "id": "27330199-57f3-41cd-8c1f-073175a54f75",
          "name": "update-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8918bd79-06f7-4d51-9d57-b9cce8d8b2b3"
            }
          ]
        },
        {
          "id": "7b0dbd83-c098-46f9-8811-0721958ac1d3",
          "name": "list-migration-systems",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/content_migrations/migrators"
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
            "description": "List migration systems."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "73b36037-0892-4a9e-b5c0-05646d4336f7"
            }
          ]
        },
        {
          "id": "afda6fbc-91a7-4421-bc7c-c47b539284e6",
          "name": "list-discussion-topics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics"
              ],
              "query": [
                {
                  "key": "only_announcements",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "order_by",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "scope",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search_term",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "List discussion topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76540d6b-593b-43f8-9732-0dad29e1e2f7"
            }
          ]
        },
        {
          "id": "36aed078-8715-43aa-b785-f0ca62e43bb1",
          "name": "create-a-new-discussion-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics"
              ],
              "query": [
                {
                  "key": "allow_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "delayed_post_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "discussion_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_announcement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "only_graders_can_rate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pinned",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_enabled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_has_student_posts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "published",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "require_initial_post",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_by_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new discussion topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "853cb907-d229-4ea6-966a-029dfd39ccb0"
            }
          ]
        },
        {
          "id": "0db511f3-d0f3-43ce-a2a2-6ddc89bccdce",
          "name": "reorder-pinned-topics",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/reorder"
              ],
              "query": [
                {
                  "key": "order",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Reorder pinned topics."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a68aea02-79e5-4d8b-8165-bf1011bb3116"
            }
          ]
        },
        {
          "id": "a96a556f-4457-44d2-a172-8f564f0dfdc6",
          "name": "get-a-single-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
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
            "description": "Get a single topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85066102-d147-45ac-8ef0-1cbe8ec8c7d1"
            }
          ]
        },
        {
          "id": "b020eb7e-a10b-45f5-b989-cf7ae1076258",
          "name": "update-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
              ],
              "query": [
                {
                  "key": "allow_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "assignment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "delayed_post_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "discussion_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "group_category_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "is_announcement",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lock_at",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "only_graders_can_rate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pinned",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_enabled",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "podcast_has_student_posts",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position_after",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "published",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "require_initial_post",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort_by_rating",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46a3b796-7438-4f68-857e-97d844a1d250"
            }
          ]
        },
        {
          "id": "33ab53b4-beff-4331-8aaf-d0be5c850ced",
          "name": "delete-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id"
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
            "description": "Delete a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8adef4fc-28b4-43e0-a679-cee1cd73778a"
            }
          ]
        },
        {
          "id": "9eb2be4a-255b-4cff-a751-923f8f4268a3",
          "name": "list-topic-entries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries"
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
            "description": "List topic entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "284f36ab-cffd-4bc1-bbe9-5ebef719c280"
            }
          ]
        },
        {
          "id": "fdd6c17b-1237-4226-9943-afff2560ab4f",
          "name": "post-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries"
              ],
              "query": [
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "523f14db-887a-467f-b087-3b3291e9652f"
            }
          ]
        },
        {
          "id": "f6aab5f1-488f-463c-9391-61ce52433769",
          "name": "rate-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/rating"
              ],
              "query": [
                {
                  "key": "rating",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Rate entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50c49a56-3518-4b2e-98ef-48086c19d336"
            }
          ]
        },
        {
          "id": "ae8fbdca-1cba-4b6c-a30e-ceab136bfc8a",
          "name": "mark-entry-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/read"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark entry as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "810728b3-2a0b-4bd1-92db-29e7c93cc15c"
            }
          ]
        },
        {
          "id": "d0c83024-84a1-450c-98f3-545f69f80110",
          "name": "mark-entry-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/read"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Mark entry as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5ebd74d-fb71-49da-a1fb-2a7cf56df251"
            }
          ]
        },
        {
          "id": "44d201ab-a978-49c2-a7a1-ffde0f87c3e9",
          "name": "list-entry-replies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/replies"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List entry replies."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "955107ef-e4c1-4073-aa21-707b0f46d734"
            }
          ]
        },
        {
          "id": "8fcd089f-18dc-48a6-a3c5-02285f0c5080",
          "name": "post-a-reply",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:entry_id/replies"
              ],
              "query": [
                {
                  "key": "attachment",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
                {
                  "id": "entry_id",
                  "value": "entry_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post a reply."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6a69a4f-0061-4b27-af72-146a00c05b23"
            }
          ]
        },
        {
          "id": "4901e8ac-c29f-475f-b2a0-6f67c8062b0d",
          "name": "update-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:id"
              ],
              "query": [
                {
                  "key": "message",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
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
            "description": "Update an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50502aa2-62f1-4f0a-8e55-db0636aacdcf"
            }
          ]
        },
        {
          "id": "281bc5dd-161a-40a1-a289-046be69361ba",
          "name": "delete-an-entry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entries/:id"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                },
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
            "description": "Delete an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83136ede-e993-45cb-a916-a189d26b0122"
            }
          ]
        },
        {
          "id": "b36f5bab-62f2-4c14-81e6-330715d9210a",
          "name": "list-entries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/entry_list"
              ],
              "query": [
                {
                  "key": "ids",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
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
            "description": "List entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4eab68d7-6f1d-41af-a0db-71953ffc9bf5"
            }
          ]
        },
        {
          "id": "5879f70e-e774-4de8-bbf4-2ee942bcc8e9",
          "name": "mark-topic-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark topic as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04ae0a82-a977-489a-88ed-0bfd6e3b5318"
            }
          ]
        },
        {
          "id": "19dad4ad-94f8-49b2-a80d-f400b22462df",
          "name": "mark-topic-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read"
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
            "description": "Mark topic as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f0841ed-fa04-4709-aacb-60685a8fd69b"
            }
          ]
        },
        {
          "id": "adb68ef0-7b87-4272-81e6-644305fa2408",
          "name": "mark-all-entries-as-read",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read_all"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Mark all entries as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c77e656d-984d-4740-867a-b95d0d6aba53"
            }
          ]
        },
        {
          "id": "76748879-c1bd-4403-977d-86adeaa3768a",
          "name": "mark-all-entries-as-unread",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/read_all"
              ],
              "query": [
                {
                  "key": "forced_read_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Mark all entries as unread."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "600c1eb0-4a0e-4c89-be83-5077a289e152"
            }
          ]
        },
        {
          "id": "3ad234dd-2f2f-4ca8-9d2d-b95091ed5021",
          "name": "subscribe-to-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/subscribed"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Subscribe to a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3efbe670-206b-4fb4-84c0-15100ce628e7"
            }
          ]
        },
        {
          "id": "84deaad7-042a-4f00-a055-f5a70c43f2b8",
          "name": "unsubscribe-from-a-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/subscribed"
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
            "description": "Unsubscribe from a topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "790ba766-6fbf-4505-b81a-810ef7bbd040"
            }
          ]
        },
        {
          "id": "e8e73a1c-4ed0-4ce2-a5a3-bde1c197bf72",
          "name": "get-the-full-topic",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/discussion_topics/topic_id/view"
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
            "description": "Get the full topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b87e19c5-fcd6-4080-a8ea-0ac6e68fdb50"
            }
          ]
        },
        {
          "id": "3e254892-4e17-42cd-98a9-89adf8d6da92",
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
              "id": "e5ab1296-2675-4c7c-b4d4-9acd3ade02c7"
            }
          ]
        },
        {
          "id": "f71af6de-d8da-432a-a88e-f534fb4f34d0",
          "name": "create-an-external-feed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/external_feeds"
              ],
              "query": [
                {
                  "key": "header_match",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "verbosity",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an external feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "156869ef-adcb-4260-87c4-e6127799e3e2"
            }
          ]
        },
        {
          "id": "9fd0e56e-c8af-46b7-8bdd-db49c1d1db67",
          "name": "delete-an-external-feed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/external_feeds/external_feed_id"
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
            "description": "Delete an external feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d890ec3f-b94f-4c89-baa9-bf0b1908f6f8"
            }
          ]
        },
        {
          "id": "f6f6d395-57ad-446e-9311-894223a3c627",
          "name": "list-files",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/files"
              ],
              "query": [
                {
                  "key": "content_types",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "only",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "order",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "search_term",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "sort",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "List files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5d0a630-64f0-4cca-8487-b98ed307c022"
            }
          ]
        },
        {
          "id": "314af362-2c33-4005-a233-026308913c9c",
          "name": "upload-a-file",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/files"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "group_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3f58474-5555-463a-98ec-4d69bd82796c"
            }
          ]
        },
        {
          "id": "67cfef04-78d2-46e3-9944-b4d0a938ca2b",
          "name": "get-file",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "groups/:group_id/files/id"
              ],
              "query": [
                {
                  "key": "include",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                }
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
            "description": "Get file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_2