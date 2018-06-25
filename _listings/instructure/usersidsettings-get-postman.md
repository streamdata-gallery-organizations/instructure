{
  "info": {
    "name": "Instructure Canvas Users API Update user settings.",
    "_postman_id": "48e422e6-4ff1-4726-991f-3b76c849ef40",
    "description": "Update user settings..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "3f2d3584-1186-4c49-a07c-5a4c44956b15",
          "name": "list-the-activity-stream",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/activity_stream",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "431e92b4-51d6-4f33-9ff9-a57cba2b6ebd"
            }
          ]
        },
        {
          "id": "b82fcd49-3c3a-47e4-935e-70e369f24754",
          "name": "list-the-activity-stream1",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "24978426-c0c2-4acc-9912-ac9bd1cea6d8"
            }
          ]
        },
        {
          "id": "0c375f92-4238-4deb-98db-14a7ea0be6b2",
          "name": "hide-all-stream-items",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Hide all stream items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "071bc59e-db5b-49d3-b4a4-0af7dbf7a783"
            }
          ]
        },
        {
          "id": "b3fb8b26-9459-4ceb-a63a-f14a9e1a0eb5",
          "name": "activity-stream-summary",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream/summary",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "96702445-8058-4b40-96b0-4f9f62a09202"
            }
          ]
        },
        {
          "id": "e6bfea0f-8324-48d2-a5ec-296e01a95b34",
          "name": "hide-a-stream-item",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/activity_stream/:id"
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
            "description": "Hide a stream item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c35bd66d-107a-43ce-bade-96b766c873d2"
            }
          ]
        },
        {
          "id": "3594ebc0-ff38-45d3-9e06-405a52cd6233",
          "name": "list-bookmarks",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/bookmarks",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List bookmarks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62eeea11-f51f-46f5-bcf7-923de8bf5249"
            }
          ]
        },
        {
          "id": "c97eda3a-fd19-4cdb-b527-6ada472c8d98",
          "name": "create-bookmark",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/bookmarks?data=%7B%7D&name=%7B%7D&position=%7B%7D&url=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb65d53c-8be3-418d-abf6-9c4f146b9599"
            }
          ]
        },
        {
          "id": "732f65eb-65c4-42ae-b61c-a7674989c81c",
          "name": "get-bookmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/bookmarks/:id"
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
            "description": "Get bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ddc00d06-f9e7-4b3e-a0dd-7352a94d461c"
            }
          ]
        },
        {
          "id": "024a4cd9-e06f-4732-b847-d2ea23ae1aed",
          "name": "update-bookmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/bookmarks/:id"
              ],
              "query": [
                {
                  "key": "data",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Update bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44a06481-bb36-49a9-807a-1750643d46e7"
            }
          ]
        },
        {
          "id": "d4be85bc-5bea-45dd-bfbd-ec108094c1d8",
          "name": "delete-bookmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/bookmarks/:id"
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
            "description": "Delete bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b071afb2-4c56-4c37-a6a1-adde523b486b"
            }
          ]
        },
        {
          "id": "faa71c47-da6e-4598-8daa-3a5a0397ae3b",
          "name": "update-multiple-preferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:communication_channel_id/notification_preferences"
              ],
              "query": [
                {
                  "key": "notification_preferences[X][frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "communication_channel_id",
                  "value": "communication_channel_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update multiple preferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6278dbda-d339-4303-8299-9ff783315e73"
            }
          ]
        },
        {
          "id": "86853feb-992c-407b-9278-4bd3647fbcb0",
          "name": "update-a-preference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:communication_channel_id/notification_preferences/notification"
              ],
              "query": [
                {
                  "key": "notification_preferences[frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "communication_channel_id",
                  "value": "communication_channel_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a preference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88175000-f12b-4c4d-beb1-0c151845aa8e"
            }
          ]
        },
        {
          "id": "4111e1a8-15af-4310-8405-2faa85baaff5",
          "name": "update-preferences-by-category",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:communication_channel_id/notification_preference_categories/category"
              ],
              "query": [
                {
                  "key": "category",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "notification_preferences[frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "communication_channel_id",
                  "value": "communication_channel_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update preferences by category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c87df6a4-d553-430e-92a2-0ce0ce9ce86d"
            }
          ]
        },
        {
          "id": "aa66cce6-04c2-4e40-a103-6246f424a847",
          "name": "update-multiple-preferences1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:type/address/notification_preferences"
              ],
              "query": [
                {
                  "key": "notification_preferences[X][frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "type",
                  "value": "type",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update multiple preferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "335e4892-1679-47c6-a8dd-1f389bfdb408"
            }
          ]
        },
        {
          "id": "524ff392-7120-48f5-a14e-f732ca7c52c2",
          "name": "update-a-preference1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:type/address/notification_preferences/:notification"
              ],
              "query": [
                {
                  "key": "notification_preferences[frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "type",
                  "value": "type",
                  "type": "string"
                },
                {
                  "id": "notification",
                  "value": "notification",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a preference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcf90b6d-0ab0-40e7-b20f-7a8d7cfb96a2"
            }
          ]
        },
        {
          "id": "a7bcec8d-05ce-4d5a-acbf-b0a615ef3827",
          "name": "list-course-nicknames",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/course_nicknames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List course nicknames."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6da13aa4-be9e-4664-8c53-08b1cd0d4914"
            }
          ]
        },
        {
          "id": "33681565-16b0-48cf-81ca-18291f891ae0",
          "name": "clear-course-nicknames",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/course_nicknames",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Clear course nicknames."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db67cad7-444d-4ec9-a566-8e0049d6c0a0"
            }
          ]
        },
        {
          "id": "03cc5bf9-d943-4c1d-b314-ab49769b42ef",
          "name": "get-course-nickname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/course_nicknames/:course_id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get course nickname."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2d4991f-f462-4ff9-871e-6fd4e81ea5dc"
            }
          ]
        },
        {
          "id": "d4cb824c-c8dd-46f5-978f-b5ccb9d5ccb7",
          "name": "set-course-nickname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/course_nicknames/:course_id"
              ],
              "query": [
                {
                  "key": "nickname",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Set course nickname."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7837f1d-31f6-4b7f-9692-9a6363b67a41"
            }
          ]
        },
        {
          "id": "6462aea7-a22e-4d99-9128-aeddb3e96c8e",
          "name": "remove-course-nickname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/course_nicknames/:course_id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove course nickname."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36053ba9-cb8a-4eaf-8f19-6f1700e37eb3"
            }
          ]
        },
        {
          "id": "2c2cc939-ed2f-48ab-a1b7-f7f8649f6c5d",
          "name": "list-favorite-courses",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/courses",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List favorite courses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a991006-29fb-4552-9900-bc923c5633c3"
            }
          ]
        },
        {
          "id": "e2e7fe77-76a9-4988-8937-6f66306b3b34",
          "name": "reset-course-favorites",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/courses",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Reset course favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b34d9ac2-dab2-4c0f-a542-309640094ad9"
            }
          ]
        },
        {
          "id": "278fb206-0d9a-4d93-b7ec-21413804d41a",
          "name": "add-course-to-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/courses/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add course to favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bc95626-bf7e-4af7-b745-619fb5563aff"
            }
          ]
        },
        {
          "id": "e8ee5e49-137b-4017-91f2-bcf94a7ffb35",
          "name": "remove-course-from-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/courses/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove course from favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "446b8c4f-56e9-4dfc-9b85-587792280c94"
            }
          ]
        },
        {
          "id": "1aec6007-7ed7-4b9d-9794-411bc5b9dad8",
          "name": "list-favorite-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/groups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List favorite groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "185abcc5-81cd-4353-8948-dd5f20780075"
            }
          ]
        },
        {
          "id": "ac322ced-926a-43cc-a5b7-4b41fb9e9aa2",
          "name": "reset-group-favorites",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/groups",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Reset group favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3493612-b36d-429a-920a-87b51a5ba569"
            }
          ]
        },
        {
          "id": "e2a563b5-354f-422a-a1fc-effd6d270085",
          "name": "add-group-to-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add group to favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36fd2be8-3849-4e9e-9633-aae4e5913df6"
            }
          ]
        },
        {
          "id": "0f8982ee-c5fd-480e-b853-6599b0e40913",
          "name": "remove-group-from-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove group from favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afebc780-13a2-44be-a91b-1a8b3eb3cf40"
            }
          ]
        },
        {
          "id": "41741d30-7a65-47a6-94ca-7f63ec710f77",
          "name": "list-your-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/groups?context_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List your groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2947405a-f1f2-485e-a8c5-d3d0cf0c3964"
            }
          ]
        },
        {
          "id": "e49b5901-87f1-49d9-a7ad-50925080f2bb",
          "name": "list-the-todo-items",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/todo",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the todo items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1541d30d-0021-4976-9e41-3ef5f6cb9992"
            }
          ]
        },
        {
          "id": "9a5f2fe4-485e-4fc4-88f6-a481a63c59f5",
          "name": "list-upcoming-assignments-calendar-events",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/upcoming_events",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List upcoming assignments, calendar events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1c256f1-6fd8-49be-a6ed-21867c586831"
            }
          ]
        },
        {
          "id": "40a67490-52e4-4e29-923d-5eae0a454f2f",
          "name": "show-user-details",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id"
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
            "description": "Show user details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1fc0e9f1-4372-409e-a9e3-9201f0cfef04"
            }
          ]
        },
        {
          "id": "35478c46-6cd6-44f0-9695-4c0fad653763",
          "name": "edit-a-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id"
              ],
              "query": [
                {
                  "key": "user[avatar][token]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[avatar][url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[email]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[locale]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[short_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[sortable_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[time_zone]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Edit a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0628a21f-4ed8-4acf-888b-aa33ec8b3ccb"
            }
          ]
        },
        {
          "id": "4ce380dd-234f-43fb-b83f-5ea2d66efeb8",
          "name": "get-custom-colors",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/colors"
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
            "description": "Get custom colors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5f64ffd-53da-48fd-863c-69478e91876f"
            }
          ]
        },
        {
          "id": "3f530028-9961-4071-8f95-cc775bd23121",
          "name": "get-custom-color",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/colors/asset_string"
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
            "description": "Get custom color."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97509ae4-fb39-495f-a7a5-f7182a7a5ebb"
            }
          ]
        },
        {
          "id": "ae19cb5d-f9e6-4b74-81ff-f9211238b164",
          "name": "update-custom-color",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/colors/asset_string"
              ],
              "query": [
                {
                  "key": "hexcode",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
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
            "description": "Update custom color."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdbeb045-cf46-4ce4-b3b0-9ede22765503"
            }
          ]
        },
        {
          "id": "d8f1ece2-18b7-4de0-adee-e7968ef33b02",
          "name": "merge-user-into-another-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/merge_into/accounts/destination_account_id/users/:destination_user_id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "destination_user_id",
                  "value": "destination_user_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Merge user into another user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5116eaeb-e612-461c-b27c-3107f32ae822"
            }
          ]
        },
        {
          "id": "13e28615-e3d3-47a8-9c7f-7afce8819972",
          "name": "merge-user-into-another-user1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/merge_into/destination_user_id"
              ],
              "variable": [
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
            "description": "Merge user into another user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "490a8cd2-5f12-4bc6-9cee-7b5ac089a6dd"
            }
          ]
        },
        {
          "id": "e21c6f5b-c34c-4804-86fb-2c49e285646d",
          "name": "update-user-settings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/settings"
              ],
              "query": [
                {
                  "key": "manual_mark_as_read",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Update user settings.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5076cbab-2583-421f-a5ee-1505d905bf78"
            }
          ]
        }
      ]
    }
  ]
}