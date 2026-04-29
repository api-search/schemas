---
description: UploadOptions schema from Amplitude HTTP V2 API
layout: schema
name: UploadOptions
properties_list:
- description: Minimum length for user_id and device_id fields. Default is 5.
  name: min_id_length
  type: integer
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/http-v2-api-upload-options-schema.json
slug: http-v2-api-upload-options
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/http-v2-api-upload-options-schema.json\",\n  \"title\": \"UploadOptions\",\n  \"description\": \"UploadOptions schema from Amplitude HTTP V2 API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"min_id_length\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum length for user_id and device_id fields. Default is 5.\",\n      \"minimum\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/http-v2-api-upload-options-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UploadOptions
---
