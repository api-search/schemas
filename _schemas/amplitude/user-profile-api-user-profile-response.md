---
description: UserProfileResponse schema from Amplitude User Profile API
layout: schema
name: UserProfileResponse
properties_list:
- description: ''
  name: userData
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/user-profile-api-user-profile-response-schema.json
slug: user-profile-api-user-profile-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-profile-api-user-profile-response-schema.json\",\n  \"title\": \"UserProfileResponse\",\n  \"description\": \"UserProfileResponse schema from Amplitude User Profile API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"userData\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"user_id\": {\n          \"type\": \"string\",\n          \"description\": \"The user's user_id.\"\n        },\n        \"user_properties\": {\n          \"type\": \"object\",\n          \"description\": \"A dictionary of the user's properties as set via the Identify API or SDK.\",\n          \"additionalProperties\": true\n        },\n        \"computed_properties\": {\n          \"type\": \"object\",\n          \"description\": \"A dictionary of computed properties calculated by Amplitude for the user.\"\
  ,\n          \"additionalProperties\": true\n        },\n        \"cohort_ids\": {\n          \"type\": \"array\",\n          \"description\": \"Array of cohort IDs the user is a member of.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"recommendations\": {\n          \"type\": \"array\",\n          \"description\": \"Array of personalized recommendation results for the user. Only included when get_recs is true.\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/Recommendation\"\n          }\n        },\n        \"amplitude_id\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"description\": \"The Amplitude internal ID for the user.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-profile-api-user-profile-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserProfileResponse
---
