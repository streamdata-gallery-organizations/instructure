---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API Remove usage rights
  description: Remove usage rights.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/activity_stream:
    get:
      summary: List the activity stream
      description: List the activity stream.
      operationId: list-the-activity-stream
      x-api-path-slug: usersactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Activity
      - Stream
  /users/self/activity_stream:
    delete:
      summary: Hide all stream items
      description: Hide all stream items.
      operationId: hide-all-stream-items
      x-api-path-slug: usersselfactivity-stream-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
    get:
      summary: List the activity stream
      description: List the activity stream.
      operationId: list-the-activity-stream
      x-api-path-slug: usersselfactivity-stream-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
  /users/self/activity_stream/summary:
    get:
      summary: Activity stream summary
      description: Activity stream summary.
      operationId: activity-stream-summary
      x-api-path-slug: usersselfactivity-streamsummary-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Summary
  /users/self/activity_stream/{id}:
    delete:
      summary: Hide a stream item
      description: Hide a stream item.
      operationId: hide-a-stream-item
      x-api-path-slug: usersselfactivity-streamid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Activity
      - Stream
      - Id
  /users/self/bookmarks:
    get:
      summary: List bookmarks
      description: List bookmarks.
      operationId: list-bookmarks
      x-api-path-slug: usersselfbookmarks-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
    post:
      summary: Create bookmark
      description: Create bookmark.
      operationId: create-bookmark
      x-api-path-slug: usersselfbookmarks-post
      parameters:
      - in: query
        name: data
        description: The data associated with the bookmark
      - in: query
        name: name
        description: The name of the bookmark
      - in: query
        name: position
        description: The position of the bookmark
      - in: query
        name: url
        description: The url of the bookmark
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
  /users/self/bookmarks/{id}:
    delete:
      summary: Delete bookmark
      description: Delete bookmark.
      operationId: delete-bookmark
      x-api-path-slug: usersselfbookmarksid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
    get:
      summary: Get bookmark
      description: Get bookmark.
      operationId: get-bookmark
      x-api-path-slug: usersselfbookmarksid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
    put:
      summary: Update bookmark
      description: Update bookmark.
      operationId: update-bookmark
      x-api-path-slug: usersselfbookmarksid-put
      parameters:
      - in: query
        name: data
        description: The data associated with the bookmark
      - in: query
        name: name
        description: The name of the bookmark
      - in: query
        name: position
        description: The position of the bookmark
      - in: query
        name: url
        description: The url of the bookmark
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Bookmarks
      - Id
  /users/self/communication_channels/{communication_channel_id}/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
  /users/self/communication_channels/{communication_channel_id}/notification_preferences/notification:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
      - Notification
  /users/self/communication_channels/{communication_channel_id}/notification_preference_categories/category:
    put:
      summary: Update preferences by category
      description: Update preferences by category.
      operationId: update-preferences-by-category
      x-api-path-slug: usersselfcommunication-channelscommunication-channel-idnotification-preference-categoriescategory-put
      parameters:
      - in: query
        name: category
        description: The name of the category
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for each notification in the category
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preference
      - Categories
      - Category
  /users/self/communication_channels/{type}/address/notification_preferences:
    put:
      summary: Update multiple preferences
      description: Update multiple preferences.
      operationId: update-multiple-preferences
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferences-put
      parameters:
      - in: query
        name: notification_preferences[X][frequency]
        description: The desired frequency for &lt;X&gt; notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
  /users/self/communication_channels/{type}/address/notification_preferences/{notification}:
    put:
      summary: Update a preference
      description: Update a preference.
      operationId: update-a-preference
      x-api-path-slug: usersselfcommunication-channelstypeaddressnotification-preferencesnotification-put
      parameters:
      - in: query
        name: notification_preferences[frequency]
        description: The desired frequency for this notification
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
      - Notification
  /users/self/course_nicknames:
    delete:
      summary: Clear course nicknames
      description: Clear course nicknames.
      operationId: clear-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
    get:
      summary: List course nicknames
      description: List course nicknames.
      operationId: list-course-nicknames
      x-api-path-slug: usersselfcourse-nicknames-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
  /users/self/course_nicknames/{course_id}:
    delete:
      summary: Remove course nickname
      description: Remove course nickname.
      operationId: remove-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    get:
      summary: Get course nickname
      description: Get course nickname.
      operationId: get-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
    put:
      summary: Set course nickname
      description: Set course nickname.
      operationId: set-course-nickname
      x-api-path-slug: usersselfcourse-nicknamescourse-id-put
      parameters:
      - in: query
        name: nickname
        description: The nickname to set
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Course
      - Nicknames
      - Course
      - Id
  /users/self/favorites/courses:
    delete:
      summary: Reset course favorites
      description: Reset course favorites.
      operationId: reset-course-favorites
      x-api-path-slug: usersselffavoritescourses-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
    get:
      summary: List favorite courses
      description: List favorite courses.
      operationId: list-favorite-courses
      x-api-path-slug: usersselffavoritescourses-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
  /users/self/favorites/courses/{id}:
    delete:
      summary: Remove course from favorites
      description: Remove course from favorites.
      operationId: remove-course-from-favorites
      x-api-path-slug: usersselffavoritescoursesid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the course to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
    post:
      summary: Add course to favorites
      description: Add course to favorites.
      operationId: add-course-to-favorites
      x-api-path-slug: usersselffavoritescoursesid-post
      parameters:
      - in: query
        name: id
        description: The ID or SIS ID of the course to add
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Courses
      - Id
  /users/self/favorites/groups:
    delete:
      summary: Reset group favorites
      description: Reset group favorites.
      operationId: reset-group-favorites
      x-api-path-slug: usersselffavoritesgroups-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
    get:
      summary: List favorite groups
      description: List favorite groups.
      operationId: list-favorite-groups
      x-api-path-slug: usersselffavoritesgroups-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
  /users/self/favorites/groups/{id}:
    delete:
      summary: Remove group from favorites
      description: Remove group from favorites.
      operationId: remove-group-from-favorites
      x-api-path-slug: usersselffavoritesgroupsid-delete
      parameters:
      - in: query
        name: id
        description: the ID or SIS ID of the group to remove
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
      - Id
    post:
      summary: Add group to favorites
      description: Add group to favorites.
      operationId: add-group-to-favorites
      x-api-path-slug: usersselffavoritesgroupsid-post
      parameters:
      - in: query
        name: id
        description: The ID or SIS ID of the group to add
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Favorites
      - Groups
      - Id
  /users/self/groups:
    get:
      summary: List your groups
      description: List your groups.
      operationId: list-your-groups
      x-api-path-slug: usersselfgroups-get
      parameters:
      - in: query
        name: context_type
        description: Only include groups that are in this type of context
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Groups
  /users/self/todo:
    get:
      summary: List the TODO items
      description: List the todo items.
      operationId: list-the-todo-items
      x-api-path-slug: usersselftodo-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Todo
  /users/self/upcoming_events:
    get:
      summary: List upcoming assignments, calendar events
      description: List upcoming assignments, calendar events.
      operationId: list-upcoming-assignments-calendar-events
      x-api-path-slug: usersselfupcoming-events-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Upcoming
      - Events
  /users/{id}:
    get:
      summary: Show user details
      description: Show user details.
      operationId: show-user-details
      x-api-path-slug: usersid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
    put:
      summary: Edit a user
      description: Edit a user.
      operationId: edit-a-user
      x-api-path-slug: usersid-put
      parameters:
      - in: query
        name: user[avatar][token]
        description: A unique representation of the avatar record to assign as the
          user&#39;sncurrent avatar
      - in: query
        name: user[avatar][url]
        description: To set the user&#39;s avatar to point to an external url, do
          not include antoken and instead pass the url here
      - in: query
        name: user[email]
        description: The default email address of the user
      - in: query
        name: user[locale]
        description: The user&#39;s preferred language as a two-letter ISO 639-1 code
      - in: query
        name: user[name]
        description: The full name of the user
      - in: query
        name: user[short_name]
        description: User&#39;s name as it will be displayed in discussions, messages,
          andncomments
      - in: query
        name: user[sortable_name]
        description: User&#39;s name as used to sort alphabetically in lists
      - in: query
        name: user[time_zone]
        description: The time zone for the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
  /users/{id}/colors:
    get:
      summary: Get custom colors
      description: Get custom colors.
      operationId: get-custom-colors
      x-api-path-slug: usersidcolors-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Colors
  /users/{id}/colors/asset_string:
    get:
      summary: Get custom color
      description: Get custom color.
      operationId: get-custom-color
      x-api-path-slug: usersidcolorsasset-string-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Colors
      - Asset
      - String
    put:
      summary: Update custom color
      description: Update custom color.
      operationId: update-custom-color
      x-api-path-slug: usersidcolorsasset-string-put
      parameters:
      - in: query
        name: hexcode
        description: The hexcode of the color to set for the context, if you choose
          to pass thenhexcode as a query parameter rather than in the request body
          you should NOTninclude the &#39;#&#39; unless you escape it first
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Colors
      - Asset
      - String
  /users/{id}/merge_into/accounts/destination_account_id/users/{destination_user_id}:
    put:
      summary: Merge user into another user
      description: Merge user into another user.
      operationId: merge-user-into-another-user
      x-api-path-slug: usersidmerge-intoaccountsdestination-account-idusersdestination-user-id-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Merge
      - Into
      - Accounts
      - Destination
      - Account
      - Id
      - Users
      - Destination
      - User
      - Id
  /users/{id}/merge_into/destination_user_id:
    put:
      summary: Merge user into another user
      description: Merge user into another user.
      operationId: merge-user-into-another-user
      x-api-path-slug: usersidmerge-intodestination-user-id-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Merge
      - Into
      - Destination
      - User
      - Id
  /users/{id}/settings:
    get:
      summary: Update user settings.
      description: Update user settings..
      operationId: update-user-settings
      x-api-path-slug: usersidsettings-get
      parameters:
      - in: query
        name: manual_mark_as_read
        description: If true, require user to manually mark discussion posts as read
          (don&#39;tnauto-mark as read)
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Settings
    put:
      summary: Update user settings.
      description: Update user settings..
      operationId: update-user-settings
      x-api-path-slug: usersidsettings-put
      parameters:
      - in: query
        name: manual_mark_as_read
        description: If true, require user to manually mark discussion posts as read
          (don&#39;tnauto-mark as read)
      responses:
        200:
          description: OK
      tags:
      - Users
      - Id
      - Settings
  /users/{user_id}/avatars:
    get:
      summary: List avatar options
      description: List avatar options.
      operationId: list-avatar-options
      x-api-path-slug: usersuser-idavatars-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Avatars
  /users/{user_id}/calendar_events:
    get:
      summary: List calendar events for a user
      description: List calendar events for a user.
      operationId: list-calendar-events-for-a-user
      x-api-path-slug: usersuser-idcalendar-events-get
      parameters:
      - in: query
        name: all_events
        description: Defaults to false (uses start_date, end_date, and undated criteria)
      - in: query
        name: context_codes[]
        description: List of context codes of courses/groups/users whose events you
          want to see
      - in: query
        name: end_date
        description: Only return events before the end_date (inclusive)
      - in: query
        name: excludes[]
        description: Array of attributes to exclude
      - in: query
        name: start_date
        description: Only return events since the start_date (inclusive)
      - in: query
        name: type
        description: 'Defaults to u201ceventu201dnn        n        n          Allowed
          values: event, assignment'
      - in: query
        name: undated
        description: Defaults to false (dated events only)
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Calendar
      - Events
  /users/{user_id}/communication_channels:
    get:
      summary: List user communication channels
      description: List user communication channels.
      operationId: list-user-communication-channels
      x-api-path-slug: usersuser-idcommunication-channels-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
    post:
      summary: Create a communication channel
      description: Create a communication channel.
      operationId: create-a-communication-channel
      x-api-path-slug: usersuser-idcommunication-channels-post
      parameters:
      - in: query
        name: communication_channel[address]
        description: An email address or SMS number
      - in: query
        name: communication_channel[token]
        description: A registration id, device token, or equivalent token given to
          an app whennregistering with a push notification provider
      - in: query
        name: communication_channel[type]
        description: The type of communication channel
      - in: query
        name: skip_confirmation
        description: Only valid for site admins and account admins making requests;
          If true, thenchannel is automatically validated and no confirmation email
          or SMS isnsent
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
  /users/{user_id}/communication_channels/communication_channel_id/notification_preferences:
    get:
      summary: List preferences
      description: List preferences.
      operationId: list-preferences
      x-api-path-slug: usersuser-idcommunication-channelscommunication-channel-idnotification-preferences-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
  /users/{user_id}/communication_channels/communication_channel_id/notification_preferences/{notification}:
    get:
      summary: Get a preference
      description: Get a preference.
      operationId: get-a-preference
      x-api-path-slug: usersuser-idcommunication-channelscommunication-channel-idnotification-preferencesnotification-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preferences
      - Notification
  /users/{user_id}/communication_channels/communication_channel_id/notification_preference_categories:
    get:
      summary: List of preference categories
      description: List of preference categories.
      operationId: list-of-preference-categories
      x-api-path-slug: usersuser-idcommunication-channelscommunication-channel-idnotification-preference-categories-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Communication
      - Channel
      - Id
      - Notification
      - Preference
      - Categories
  /users/{user_id}/communication_channels/id:
    delete:
      summary: Delete a communication channel
      description: Delete a communication channel.
      operationId: delete-a-communication-channel
      x-api-path-slug: usersuser-idcommunication-channelsid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Id
  /users/{user_id}/communication_channels/type/{address}:
    delete:
      summary: Delete a communication channel
      description: Delete a communication channel.
      operationId: delete-a-communication-channel
      x-api-path-slug: usersuser-idcommunication-channelstypeaddress-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Type
      - Address
  /users/{user_id}/communication_channels/type/{address}/notification_preferences:
    get:
      summary: List preferences
      description: List preferences.
      operationId: list-preferences
      x-api-path-slug: usersuser-idcommunication-channelstypeaddressnotification-preferences-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
  /users/{user_id}/communication_channels/type/{address}/notification_preferences/notification:
    get:
      summary: Get a preference
      description: Get a preference.
      operationId: get-a-preference
      x-api-path-slug: usersuser-idcommunication-channelstypeaddressnotification-preferencesnotification-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Communication
      - Channels
      - Type
      - Address
      - Notification
      - Preferences
      - Notification
  /users/{user_id}/content_exports:
    get:
      summary: List content exports
      description: List content exports.
      operationId: list-content-exports
      x-api-path-slug: usersuser-idcontent-exports-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Exports
    post:
      summary: Export content
      description: Export content.
      operationId: export-content
      x-api-path-slug: usersuser-idcontent-exports-post
      parameters:
      - in: query
        name: export_type
        description: u201ccommon_cartridgeu201dnnExport the contents of the course
          in the Common Cartridge (
      - in: query
        name: skip_notifications
        description: Don&#39;t send the notifications about the export to the user
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Exports
  /users/{user_id}/content_exports/id:
    get:
      summary: Show content export
      description: Show content export.
      operationId: show-content-export
      x-api-path-slug: usersuser-idcontent-exportsid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Exports
      - Id
  /users/{user_id}/content_licenses:
    get:
      summary: List licenses
      description: List licenses.
      operationId: list-licenses
      x-api-path-slug: usersuser-idcontent-licenses-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Licenses
  /users/{user_id}/content_migrations:
    get:
      summary: List content migrations
      description: List content migrations.
      operationId: list-content-migrations
      x-api-path-slug: usersuser-idcontent-migrations-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Migrations
    post:
      summary: Create a content migration
      description: Create a content migration.
      operationId: create-a-content-migration
      x-api-path-slug: usersuser-idcontent-migrations-post
      parameters:
      - in: query
        name: date_shift_options[day_substitutions][X]
        description: Move anything scheduled for day &#39;X&#39; to the specified
          day
      - in: query
        name: date_shift_options[new_end_date]
        description: The new end date for the source content/course
      - in: query
        name: date_shift_options[new_start_date]
        description: The new start date for the content/course
      - in: query
        name: date_shift_options[old_end_date]
        description: The original end date of the source content/course
      - in: query
        name: date_shift_options[old_start_date]
        description: The original start date of the source content/course
      - in: query
        name: date_shift_options[remove_dates]
        description: Whether to remove dates in the copied course
      - in: query
        name: date_shift_options[shift_dates]
        description: Whether to shift dates in the copied course
      - in: query
        name: migration_type
        description: The type of the migration
      - in: query
        name: pre_attachment[*]
        description: Other file upload properties, See File Upload Documentation
      - in: query
        name: pre_attachment[name]
        description: Required if uploading a file
      - in: query
        name: settings[file_url]
        description: A URL to download the file from
      - in: query
        name: settings[folder_id]
        description: 'The folder to unzip the '
      - in: query
        name: settings[overwrite_quizzes]
        description: Whether to overwrite quizzes with the same identifiers between
          contentnpackages
      - in: query
        name: settings[question_bank_id]
        description: The existing question bank ID to import questions into if not
          specified innthe content package
      - in: query
        name: settings[question_bank_name]
        description: The question bank to import questions into if not specified in
          the contentnpackage, if both bank id and name are set, id will take precedence
      - in: query
        name: settings[source_course_id]
        description: The course to copy from for a course copy migration
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Migrations
  /users/{user_id}/content_migrations/content_migration_id/migration_issues:
    get:
      summary: List migration issues
      description: List migration issues.
      operationId: list-migration-issues
      x-api-path-slug: usersuser-idcontent-migrationscontent-migration-idmigration-issues-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
  /users/{user_id}/content_migrations/content_migration_id/migration_issues/{id}:
    get:
      summary: Get a migration issue
      description: Get a migration issue.
      operationId: get-a-migration-issue
      x-api-path-slug: usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
      - Id
    put:
      summary: Update a migration issue
      description: Update a migration issue.
      operationId: update-a-migration-issue
      x-api-path-slug: usersuser-idcontent-migrationscontent-migration-idmigration-issuesid-put
      parameters:
      - in: query
        name: workflow_state
        description: Set the workflow_state of the issue
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Migrations
      - Content
      - Migration
      - Id
      - Migration
      - Issues
      - Id
  /users/{user_id}/content_migrations/id:
    get:
      summary: Get a content migration
      description: Get a content migration.
      operationId: get-a-content-migration
      x-api-path-slug: usersuser-idcontent-migrationsid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Migrations
      - Id
    put:
      summary: Update a content migration
      description: Update a content migration.
      operationId: update-a-content-migration
      x-api-path-slug: usersuser-idcontent-migrationsid-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Migrations
      - Id
  /users/{user_id}/content_migrations/migrators:
    get:
      summary: List Migration Systems
      description: List migration systems.
      operationId: list-migration-systems
      x-api-path-slug: usersuser-idcontent-migrationsmigrators-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Content
      - Migrations
      - Migrators
  /users/{user_id}/courses:
    get:
      summary: List courses for a user
      description: List courses for a user.
      operationId: list-courses-for-a-user
      x-api-path-slug: usersuser-idcourses-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cneeds_grading_countu201d: Optional information to include
          with each Course'
      - in: query
        name: state[]
        description: If set, only return courses that are in the given state(s)
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Courses
  /users/{user_id}/courses/course_id/assignments:
    get:
      summary: List assignments for user
      description: List assignments for user.
      operationId: list-assignments-for-user
      x-api-path-slug: usersuser-idcoursescourse-idassignments-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Courses
      - Course
      - Id
      - Assignments
  /users/{user_id}/custom_data(/*scope):
    delete:
      summary: Delete custom data
      description: Delete custom data.
      operationId: delete-custom-data
      x-api-path-slug: usersuser-idcustom-datascope-delete
      parameters:
      - in: query
        name: ns
        description: The namespace from which to delete the data
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Custom
      - Data(
      - '*scope)'
    get:
      summary: Load custom data
      description: Load custom data.
      operationId: load-custom-data
      x-api-path-slug: usersuser-idcustom-datascope-get
      parameters:
      - in: query
        name: ns
        description: The namespace from which to retrieve the data
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Custom
      - Data(
      - '*scope)'
    put:
      summary: Store custom data
      description: Store custom data.
      operationId: store-custom-data
      x-api-path-slug: usersuser-idcustom-datascope-put
      parameters:
      - in: query
        name: data
        description: The data you want to store for the user, at the specified scope
      - in: query
        name: ns
        description: The namespace under which to store the data
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Custom
      - Data(
      - '*scope)'
  /users/{user_id}/enrollments:
    get:
      summary: List enrollments
      description: List enrollments.
      operationId: list-enrollments
      x-api-path-slug: usersuser-idenrollments-get
      parameters:
      - in: query
        name: grading_period_id
        description: Return grades for the given grading_period
      - in: query
        name: role[]
        description: A list of enrollment roles to return
      - in: query
        name: state[]
        description: Filter by enrollment state
      - in: query
        name: type[]
        description: A list of enrollment types to return
      - in: query
        name: user_id
        description: Filter by user_id (only valid for course or section enrollment
          queries)
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Enrollments
  /users/{user_id}/features:
    get:
      summary: List features
      description: List features.
      operationId: list-features
      x-api-path-slug: usersuser-idfeatures-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
  /users/{user_id}/features/enabled:
    get:
      summary: List enabled features
      description: List enabled features.
      operationId: list-enabled-features
      x-api-path-slug: usersuser-idfeaturesenabled-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
      - Enabled
  /users/{user_id}/features/flags/feature:
    delete:
      summary: Remove feature flag
      description: Remove feature flag.
      operationId: remove-feature-flag
      x-api-path-slug: usersuser-idfeaturesflagsfeature-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
      - Flags
      - Feature
    get:
      summary: Get feature flag
      description: Get feature flag.
      operationId: get-feature-flag
      x-api-path-slug: usersuser-idfeaturesflagsfeature-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
      - Flags
      - Feature
    put:
      summary: Set feature flag
      description: Set feature flag.
      operationId: set-feature-flag
      x-api-path-slug: usersuser-idfeaturesflagsfeature-put
      parameters:
      - in: query
        name: locking_account_id
        description: If set, this FeatureFlag may only be modified by someone withnadministrative
          rights in the specified account
      - in: query
        name: state
        description: u201coffu201dnnThe feature is not available for the course, user,
          or account andnsub-accounts
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Features
      - Flags
      - Feature
  /users/{user_id}/files:
    get:
      summary: List files
      description: List files.
      operationId: list-files
      x-api-path-slug: usersuser-idfiles-get
      parameters:
      - in: query
        name: content_types[]
        description: Filter results by content-type
      - in: query
        name: include[]
        description: Array of additional information to include
      - in: query
        name: only[]
        description: Array of information to restrict to
      - in: query
        name: order
        description: The sorting order
      - in: query
        name: search_term
        description: The partial name of the files to match and return
      - in: query
        name: sort
        description: Sort results by this field
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
    post:
      summary: Upload a file
      description: Upload a file.
      operationId: upload-a-file
      x-api-path-slug: usersuser-idfiles-post
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
  /users/{user_id}/files/id:
    get:
      summary: Get file
      description: Get file.
      operationId: get-file
      x-api-path-slug: usersuser-idfilesid-get
      parameters:
      - in: query
        name: include[]
        description: Array of additional information to include
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
      - Id
  /users/{user_id}/files/quota:
    get:
      summary: Get quota information
      description: Get quota information.
      operationId: get-quota-information
      x-api-path-slug: usersuser-idfilesquota-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Files
      - Quota
  /users/{user_id}/folders:
    get:
      summary: List all folders
      description: List all folders.
      operationId: list-all-folders
      x-api-path-slug: usersuser-idfolders-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Folders
    post:
      summary: Create folder
      description: Create folder.
      operationId: create-folder
      x-api-path-slug: usersuser-idfolders-post
      parameters:
      - in: query
        name: hidden
        description: Flag the folder as hidden
      - in: query
        name: locked
        description: Flag the folder as locked
      - in: query
        name: lock_at
        description: The datetime to lock the folder at
      - in: query
        name: name
        description: The name of the folder
      - in: query
        name: parent_folder_id
        description: The id of the folder to store the file in
      - in: query
        name: parent_folder_path
        description: The path of the folder to store the new folder in
      - in: query
        name: position
        description: Set an explicit sort position for the folder
      - in: query
        name: unlock_at
        description: The datetime to unlock the folder at
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Folders
  /users/{user_id}/folders/by_path:
    get:
      summary: Resolve path
      description: Resolve path.
      operationId: resolve-path
      x-api-path-slug: usersuser-idfoldersby-path-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Folders
      - By
      - Path
  /users/{user_id}/folders/by_path/*full_path:
    get:
      summary: Resolve path
      description: Resolve path.
      operationId: resolve-path
      x-api-path-slug: usersuser-idfoldersby-pathfull-path-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Folders
      - By
      - Path
      - '*full'
      - Path
  /users/{user_id}/folders/id:
    get:
      summary: Get folder
      description: Get folder.
      operationId: get-folder
      x-api-path-slug: usersuser-idfoldersid-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Folders
      - Id
  /users/{user_id}/logins:
    get:
      summary: List user logins
      description: List user logins.
      operationId: list-user-logins
      x-api-path-slug: usersuser-idlogins-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Logins
  /users/{user_id}/logins/id:
    delete:
      summary: Delete a user login
      description: Delete a user login.
      operationId: delete-a-user-login
      x-api-path-slug: usersuser-idloginsid-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Logins
      - Id
  /users/{user_id}/missing_submissions:
    get:
      summary: List Missing Submissions
      description: List missing submissions.
      operationId: list-missing-submissions
      x-api-path-slug: usersuser-idmissing-submissions-get
      parameters:
      - in: query
        name: user_id
        description: the student&#39;s ID
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Missing
      - Submissions
  /users/{user_id}/observees:
    get:
      summary: List observees
      description: List observees.
      operationId: list-observees
      x-api-path-slug: usersuser-idobservees-get
      parameters:
      - in: query
        name: include[]
        description: 'u201cavatar_urlu201d: Optionally include avatar_url'
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Observees
    post:
      summary: Add an observee with credentials
      description: Add an observee with credentials.
      operationId: add-an-observee-with-credentials
      x-api-path-slug: usersuser-idobservees-post
      parameters:
      - in: query
        name: access_token
        description: The access token for the user to observe
      - in: query
        name: observee[password]
        description: The password for the user to observe
      - in: query
        name: observee[unique_id]
        description: The login id for the user to observe
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Observees
  /users/{user_id}/observees/observee_id:
    delete:
      summary: Remove an observee
      description: Remove an observee.
      operationId: remove-an-observee
      x-api-path-slug: usersuser-idobserveesobservee-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Observees
      - Observee
      - Id
    get:
      summary: Show an observee
      description: Show an observee.
      operationId: show-an-observee
      x-api-path-slug: usersuser-idobserveesobservee-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Observees
      - Observee
      - Id
    put:
      summary: Add an observee
      description: Add an observee.
      operationId: add-an-observee
      x-api-path-slug: usersuser-idobserveesobservee-id-put
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Observees
      - Observee
      - Id
  /users/{user_id}/page_views:
    get:
      summary: List user page views
      description: List user page views.
      operationId: list-user-page-views
      x-api-path-slug: usersuser-idpage-views-get
      parameters:
      - in: query
        name: end_time
        description: The end of the time range from which you want page views
      - in: query
        name: start_time
        description: The beginning of the time range from which you want page views
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Page
      - Views
  /users/{user_id}/profile:
    get:
      summary: Get user profile
      description: Get user profile.
      operationId: get-user-profile
      x-api-path-slug: usersuser-idprofile-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Profile
  /users/{user_id}/usage_rights:
    delete:
      summary: Remove usage rights
      description: Remove usage rights.
      operationId: remove-usage-rights
      x-api-path-slug: usersuser-idusage-rights-delete
      parameters:
      - in: query
        name: file_ids[]
        description: List of ids of files to remove associated usage rights from
      - in: query
        name: folder_ids[]
        description: List of ids of folders
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Usage
      - Rights
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---