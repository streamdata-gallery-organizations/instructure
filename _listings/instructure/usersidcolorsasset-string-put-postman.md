{
  "info": {
    "name": "Instructure Canvas Users API Update custom color",
    "_postman_id": "49134fe5-cb8f-4e55-afe8-00976ba4c182",
    "description": "Update custom color.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "225e0019-2a0b-4e7c-b1c2-0eac6853c4eb",
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
              "id": "c66edfcb-7e71-48d1-a3d7-4a8035c92545"
            }
          ]
        },
        {
          "id": "4ba413f2-c06d-4a4d-b18f-60fbdff4b703",
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
              "id": "2b682743-0c8d-4510-a896-61869597aa89"
            }
          ]
        },
        {
          "id": "5112cf2a-62fe-4ef2-b8d8-c58a1b60ee34",
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
              "id": "cb4ebed5-c564-41a1-8d17-94aaa1f0f67f"
            }
          ]
        },
        {
          "id": "ceff0def-cdbf-4f1e-a8f9-c592f09d53d6",
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
              "id": "d3e37d82-ad69-4cdd-9361-184130a51cfc"
            }
          ]
        },
        {
          "id": "0cbba0a4-503e-4375-888a-60e9dfe82765",
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
              "id": "caee0980-cefb-4173-b6fe-0c0d14c8e611"
            }
          ]
        },
        {
          "id": "65be7dd2-9b9d-4b29-b9aa-37b59275d8cb",
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
              "id": "0803d5cb-a29b-4cd1-b296-b920e2af079c"
            }
          ]
        },
        {
          "id": "ae500d3c-1ba1-4134-80de-765478f16704",
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
              "id": "11c57a90-7485-4ace-81e0-8f45ae466d5b"
            }
          ]
        },
        {
          "id": "d20796fd-8e94-48a6-bfef-a95260653d76",
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
              "id": "9c2ffbd6-3ccb-4b83-8d94-ae7a85a014dd"
            }
          ]
        },
        {
          "id": "6e8bd762-4927-4d8f-b1d6-0165e363f97b",
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
              "id": "4f49a981-c05f-4ebf-8aa7-98ede28a453e"
            }
          ]
        },
        {
          "id": "8a470dd1-94dd-4656-bd17-9abd07dc57b7",
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
              "id": "e0734a59-19f1-4072-8f17-ba6a09a65b83"
            }
          ]
        },
        {
          "id": "22b6d1cd-1d13-4872-94f6-159b43a49216",
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
              "id": "6cc63380-6175-498a-b89e-1c828bbeb1d2"
            }
          ]
        },
        {
          "id": "2e111bd8-3988-4a78-955b-d1f111849e0e",
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
              "id": "234a3794-b387-4e22-8a58-b3fbe67f1adb"
            }
          ]
        },
        {
          "id": "b3b5343d-58c9-4f32-a989-ca8ca3915cd4",
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
              "id": "31ddc3c2-5897-4b25-a186-9c44966294a8"
            }
          ]
        },
        {
          "id": "bef7406b-dcb6-46f2-8367-c9fe9a932ea0",
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
              "id": "f538a870-91ec-4767-bb15-bcf16e91a5be"
            }
          ]
        },
        {
          "id": "33890dcb-507f-426f-8981-b865cd7cfcbd",
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
              "id": "820da357-469b-4b2d-9651-dc62ca06b787"
            }
          ]
        },
        {
          "id": "712a6248-e0e6-490c-acb0-3c4209600374",
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
              "id": "7dc83a91-4c53-4cd4-9e52-8c616228e1e8"
            }
          ]
        },
        {
          "id": "7b98f069-6f37-43a9-baaf-c8b804a7510e",
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
              "id": "9b2f427d-5c0b-403e-836c-8cf3300e47c0"
            }
          ]
        },
        {
          "id": "1a1041c0-28f7-46d9-be84-f1dc5faa56d6",
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
              "id": "bc74c968-0b3b-4d51-837f-c6b156fc04e5"
            }
          ]
        },
        {
          "id": "277e0f75-2331-432b-8c44-468e33077669",
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
              "id": "ed50305b-c202-4b11-af58-58d6870cb61b"
            }
          ]
        },
        {
          "id": "f61897b6-5492-4cf1-9c3b-59e9e53f2974",
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
              "id": "10c3ffdd-d2dc-4476-afd9-93863b22f8ee"
            }
          ]
        },
        {
          "id": "0561f2a9-1cf8-4e96-ba53-966e0935fd96",
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
              "id": "3c6a17c7-ed2e-4b85-8842-9299ef4eba50"
            }
          ]
        },
        {
          "id": "ae05d1fe-b643-485f-bf89-d3e9c34b449d",
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
              "id": "3b8b5b68-3e53-4917-9d86-8af7fdd72134"
            }
          ]
        },
        {
          "id": "b8021545-ce51-4231-9209-c5e00b38af1b",
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
              "id": "185d5564-1f8b-4c12-98a3-8c8223c06d66"
            }
          ]
        },
        {
          "id": "93e831af-022d-4561-889e-331c0cfb2a9b",
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
              "id": "8b2cede3-dad5-4b99-8dea-6c22a3d8a8b4"
            }
          ]
        },
        {
          "id": "a4c8efec-19b3-4ce5-9ba1-c203531f2a68",
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
              "id": "dbd7f27e-d078-4f3b-9e12-d0e24d26ba84"
            }
          ]
        },
        {
          "id": "1971cb4c-ca6d-405b-9748-e667ff469c98",
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
              "id": "257de4bd-0aa9-4315-beb5-004f1968f556"
            }
          ]
        },
        {
          "id": "ac1629b9-2666-49cc-ada7-2b62637bf6c6",
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
              "id": "31895fe0-6e7f-4979-99e8-34d1d1767e58"
            }
          ]
        },
        {
          "id": "be626883-5c19-4bb0-a3fd-b993297baa21",
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
              "id": "83647937-82ac-4e4b-8e76-048ee004a3f2"
            }
          ]
        },
        {
          "id": "e92d97e8-22bd-48fc-90d9-b2a3b516c353",
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
              "id": "cd7326e8-0134-4dbb-b5ef-463f63cbf531"
            }
          ]
        },
        {
          "id": "35a5071a-48b7-43bf-b24f-b43935cf3912",
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
              "id": "9393e943-4473-4bcc-99ea-ca418aae9b61"
            }
          ]
        },
        {
          "id": "e889c803-f573-4647-82b2-f67cdb264eb1",
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
              "id": "1fb681a8-d310-4f3d-bd32-f855bb2f45db"
            }
          ]
        },
        {
          "id": "c67c277d-3e0a-4627-b1bb-22b824c95ff0",
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
              "id": "1dad0527-f0a3-4a44-b0dc-c2b2958a6a6c"
            }
          ]
        },
        {
          "id": "2c69367e-6ec6-4d03-b1f3-1d6e7252403c",
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
              "id": "44750ad9-4772-4dd8-8a94-54ce78fce1ee"
            }
          ]
        },
        {
          "id": "3493dcec-27ef-4682-9daf-36d4b19a770a",
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
              "id": "fb3e2dc1-fa98-43e4-b23b-b1e6a32c2b68"
            }
          ]
        },
        {
          "id": "e7ff11c4-bddd-422f-becc-e0f48bb385b7",
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
              "id": "0eb6aee8-8929-48eb-b780-f499e2306ec6"
            }
          ]
        },
        {
          "id": "0fec4df6-5f4e-4b97-b65e-8c1530f60441",
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
              "id": "7d5c1210-eccc-41ea-9638-ac0edffc9248"
            }
          ]
        }
      ]
    }
  ]
}