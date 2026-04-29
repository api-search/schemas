---
description: UserData schema from Amplitude User Profile API
layout: schema
name: UserData
properties_list:
- description: The user's user_id.
  name: user_id
  type: string
- description: A dictionary of the user's properties as set via the Identify API or SDK.
  name: user_properties
  type: object
- description: A dictionary of computed properties calculated by Amplitude for the user.
  name: computed_properties
  type: object
- description: Array of cohort IDs the user is a member of.
  name: cohort_ids
  type: array
- description: Array of personalized recommendation results for the user. Only included when get_recs is true.
  name: recommendations
  type: array
- description: The Amplitude internal ID for the user.
  name: amplitude_id
  type: integer
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/user-profile-api-user-data-schema.json
slug: user-profile-api-user-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-profile-api-user-data-schema.json\",\n  \"title\": \"UserData\",\n  \"description\": \"UserData schema from Amplitude User Profile API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"The user's user_id.\"\n    },\n    \"user_properties\": {\n      \"type\": \"object\",\n      \"description\": \"A dictionary of the user's properties as set via the Identify API or SDK.\",\n      \"additionalProperties\": true\n    },\n    \"computed_properties\": {\n      \"type\": \"object\",\n      \"description\": \"A dictionary of computed properties calculated by Amplitude for the user.\",\n      \"additionalProperties\": true\n    },\n    \"cohort_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Array of cohort IDs the user is\
  \ a member of.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"recommendations\": {\n      \"type\": \"array\",\n      \"description\": \"Array of personalized recommendation results for the user. Only included when get_recs is true.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"rec_id\": {\n            \"type\": \"string\",\n            \"description\": \"The recommendation model ID.\"\n          },\n          \"child_ids\": {\n            \"type\": \"array\",\n            \"description\": \"Array of recommended item IDs.\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"is_control\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the user is in the control group for this recommendation model.\"\n          },\n          \"recommendation_type\": {\n            \"type\": \"string\",\n            \"description\": \"The type of\
  \ recommendation model.\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"The title of the recommendation.\"\n          }\n        }\n      }\n    },\n    \"amplitude_id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The Amplitude internal ID for the user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-profile-api-user-data-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserData
---
