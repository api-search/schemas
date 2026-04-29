---
description: A set of changes within a Google Analytics account or its child properties that resulted from the same cause. Common causes would be updates made in the Google Analytics UI, changes from customer support, or automatic Google Analytics system changes.
layout: schema
name: ChangeHistoryEvent
properties_list:
- description: The type of actor that made this change.
  name: actorType
  type: string
- description: Time when change was made.
  name: changeTime
  type: string
- description: A list of changes made in this change history event that fit the filters specified in SearchChangeHistoryEventsRequest.
  name: changes
  type: array
- description: If true, then the list of changes returned was filtered, and does not represent all changes that occurred in this event.
  name: changesFiltered
  type: boolean
- description: ID of this change history event. This ID is unique across Google Analytics.
  name: id
  type: string
- description: Email address of the Google account that made the change. This will be a valid email address if the actor field is set to USER, and empty otherwise. Google accounts that have been deleted will cause a
  name: userActorEmail
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/admin-api-change-history-event-schema.json
slug: admin-api-change-history-event
source_filename: admin-api-change-history-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-change-history-event-schema.json\",\n  \"title\": \"ChangeHistoryEvent\",\n  \"description\": \"A set of changes within a Google Analytics account or its child properties that resulted from the same cause. Common causes would be updates made in the Google Analytics UI, changes from customer support, or automatic Google Analytics system changes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actorType\": {\n      \"description\": \"The type of actor that made this change.\",\n      \"enum\": [\n        \"ACTOR_TYPE_UNSPECIFIED\",\n        \"USER\",\n        \"SYSTEM\",\n        \"SUPPORT\"\n      ],\n      \"type\": \"string\",\n      \"example\": \"ACTOR_TYPE_UNSPECIFIED\"\n    },\n    \"changeTime\": {\n      \"description\": \"Time when change was made.\",\n      \"format\": \"google-datetime\"\
  ,\n      \"type\": \"string\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"changes\": {\n      \"description\": \"A list of changes made in this change history event that fit the filters specified in SearchChangeHistoryEventsRequest.\",\n      \"items\": {\n        \"description\": \"A description of a change to a single Google Analytics resource.\",\n        \"properties\": {\n          \"action\": {\n            \"description\": \"The type of action that changed this resource.\",\n            \"enum\": [\n              \"ACTION_TYPE_UNSPECIFIED\",\n              \"CREATED\",\n              \"UPDATED\",\n              \"DELETED\"\n            ],\n            \"type\": \"string\",\n            \"example\": \"ACTION_TYPE_UNSPECIFIED\"\n          },\n          \"resource\": {\n            \"description\": \"Resource name of the resource whose changes are described by this entry.\",\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n\
  \          \"resourceAfterChange\": {\n            \"$ref\": \"#/components/schemas/GoogleAnalyticsAdminV1betaChangeHistoryChangeChangeHistoryResource\",\n            \"description\": \"Resource contents from after the change was made. If this resource was deleted in this change, this field will be missing.\"\n          },\n          \"resourceBeforeChange\": {\n            \"$ref\": \"#/components/schemas/GoogleAnalyticsAdminV1betaChangeHistoryChangeChangeHistoryResource\",\n            \"description\": \"Resource contents from before the change was made. If this resource was created in this change, this field will be missing.\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"changesFiltered\": {\n      \"description\": \"If true, then the list of changes returned was filtered, and does not represent all changes that occurred in this event.\",\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"id\": {\n    \
  \  \"description\": \"ID of this change history event. This ID is unique across Google Analytics.\",\n      \"type\": \"string\",\n      \"example\": \"123456\"\n    },\n    \"userActorEmail\": {\n      \"description\": \"Email address of the Google account that made the change. This will be a valid email address if the actor field is set to USER, and empty otherwise. Google accounts that have been deleted will cause an error.\",\n      \"type\": \"string\",\n      \"example\": \"user@example.com\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-change-history-event-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: ChangeHistoryEvent
---
