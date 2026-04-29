---
description: Recommendation schema from Amplitude User Profile API
layout: schema
name: Recommendation
properties_list:
- description: The recommendation model ID.
  name: rec_id
  type: string
- description: Array of recommended item IDs.
  name: child_ids
  type: array
- description: Whether the user is in the control group for this recommendation model.
  name: is_control
  type: boolean
- description: The type of recommendation model.
  name: recommendation_type
  type: string
- description: The title of the recommendation.
  name: title
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/user-profile-api-recommendation-schema.json
slug: user-profile-api-recommendation
source_filename: user-profile-api-recommendation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-profile-api-recommendation-schema.json\",\n  \"title\": \"Recommendation\",\n  \"description\": \"Recommendation schema from Amplitude User Profile API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"rec_id\": {\n      \"type\": \"string\",\n      \"description\": \"The recommendation model ID.\"\n    },\n    \"child_ids\": {\n      \"type\": \"array\",\n      \"description\": \"Array of recommended item IDs.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"is_control\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is in the control group for this recommendation model.\"\n    },\n    \"recommendation_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of recommendation model.\"\n    },\n    \"title\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The title of the recommendation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/user-profile-api-recommendation-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: Recommendation
---
