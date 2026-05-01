---
description: A session resource from the Google Fit REST API representing a time-bounded fitness activity.
layout: schema
name: Google Fit Session
properties_list:
- description: A client-generated identifier that is unique across all sessions owned by this particular user.
  name: id
  type: string
- description: A human readable name of the session.
  name: name
  type: string
- description: A description for this session.
  name: description
  type: string
- description: A start time in milliseconds since epoch, inclusive.
  name: startTimeMillis
  type: string
- description: An end time in milliseconds since epoch, inclusive.
  name: endTimeMillis
  type: string
- description: A timestamp that indicates when the session was last modified.
  name: modifiedTimeMillis
  type: string
- description: The application that created the session.
  name: application
  type: object
- description: The type of activity this session represents.
  name: activityType
  type: integer
- description: Active time in milliseconds.
  name: activeTimeMillis
  type: string
provider_name: Google Fit REST
provider_slug: google-fitness
schema_file: json-schema/fitness.json
slug: fitness
source_filename: fitness.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-fitness/refs/heads/main/json-schema/fitness.json\",\n  \"title\": \"Google Fit Session\",\n  \"description\": \"A session resource from the Google Fit REST API representing a time-bounded fitness activity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A client-generated identifier that is unique across all sessions owned by this particular user.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A human readable name of the session.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description for this session.\"\n    },\n    \"startTimeMillis\": {\n      \"type\": \"string\",\n      \"description\": \"A start time in milliseconds since epoch, inclusive.\"\n    },\n    \"endTimeMillis\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"An end time in milliseconds since epoch, inclusive.\"\n    },\n    \"modifiedTimeMillis\": {\n      \"type\": \"string\",\n      \"description\": \"A timestamp that indicates when the session was last modified.\"\n    },\n    \"application\": {\n      \"type\": \"object\",\n      \"description\": \"The application that created the session.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"packageName\": {\n          \"type\": \"string\"\n        },\n        \"version\": {\n          \"type\": \"string\"\n        },\n        \"detailsUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    },\n    \"activityType\": {\n      \"type\": \"integer\",\n      \"description\": \"The type of activity this session represents.\"\n    },\n    \"activeTimeMillis\": {\n      \"type\": \"string\",\n      \"description\": \"Active time in milliseconds.\"\n \
  \   }\n  },\n  \"required\": [\"id\", \"startTimeMillis\", \"endTimeMillis\", \"activityType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-fitness/refs/heads/main/json-schema/fitness.json
tags:
- Activity Tracking
- Fitness
- Google
- Health
- Sessions
- Wearables
- Wellness
title: Google Fit Session
---
