---
description: UserDeletionId schema from Google Analytics API
layout: schema
name: UserDeletionId
properties_list:
- description: The type of user identifier.
  name: type
  type: string
- description: The actual user identifier value corresponding to the specified type.
  name: userId
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/user-deletion-api-user-deletion-id-schema.json
slug: user-deletion-api-user-deletion-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/user-deletion-api-user-deletion-id-schema.json\",\n  \"title\": \"UserDeletionId\",\n  \"description\": \"UserDeletionId schema from Google Analytics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of user identifier.\",\n      \"enum\": [\n        \"CLIENT_ID\",\n        \"USER_ID\",\n        \"APP_INSTANCE_ID\"\n      ],\n      \"example\": \"CLIENT_ID\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"The actual user identifier value corresponding to the specified type.\",\n      \"example\": \"123456\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"userId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/user-deletion-api-user-deletion-id-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: UserDeletionId
---
