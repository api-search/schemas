---
description: UserDeletionRequest schema from Google Analytics API
layout: schema
name: UserDeletionRequest
properties_list:
- description: Resource type identifier.
  name: kind
  type: string
- description: ''
  name: id
  type: object
- description: The Web Property ID for a Universal Analytics property. Required for Universal Analytics properties.
  name: webPropertyId
  type: string
- description: The Firebase Project ID. Required for app streams using APP_INSTANCE_ID.
  name: firebaseProjectId
  type: string
- description: The GA4 property ID.
  name: propertyId
  type: string
- description: The time when the deletion request was submitted. Set by the server.
  name: deletionRequestTime
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/user-deletion-api-user-deletion-request-schema.json
slug: user-deletion-api-user-deletion-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/user-deletion-api-user-deletion-request-schema.json\",\n  \"title\": \"UserDeletionRequest\",\n  \"description\": \"UserDeletionRequest schema from Google Analytics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier.\",\n      \"default\": \"analytics#userDeletionRequest\",\n      \"readOnly\": true,\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"type\",\n        \"userId\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of user identifier.\",\n          \"enum\": [\n            \"CLIENT_ID\",\n            \"USER_ID\",\n            \"APP_INSTANCE_ID\"\
  \n          ],\n          \"example\": \"CLIENT_ID\"\n        },\n        \"userId\": {\n          \"type\": \"string\",\n          \"description\": \"The actual user identifier value corresponding to the specified type.\",\n          \"example\": \"123456\"\n        }\n      }\n    },\n    \"webPropertyId\": {\n      \"type\": \"string\",\n      \"description\": \"The Web Property ID for a Universal Analytics property. Required for Universal Analytics properties.\",\n      \"example\": \"123456\"\n    },\n    \"firebaseProjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The Firebase Project ID. Required for app streams using APP_INSTANCE_ID.\",\n      \"example\": \"123456\"\n    },\n    \"propertyId\": {\n      \"type\": \"string\",\n      \"description\": \"The GA4 property ID.\",\n      \"example\": \"123456\"\n    },\n    \"deletionRequestTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time when the deletion\
  \ request was submitted. Set by the server.\",\n      \"readOnly\": true,\n      \"example\": \"2026-04-17T12:00:00Z\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/user-deletion-api-user-deletion-request-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: UserDeletionRequest
---
