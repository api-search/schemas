---
description: Retention schema from AhaSend API
layout: schema
name: Retention
properties_list:
- description: Number of days to retain metadata
  name: metadata
  type: integer
- description: Number of days to retain data
  name: data
  type: integer
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-retention-schema.json
slug: openapi-v2-retention
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-retention-schema.json\",\n  \"title\": \"Retention\",\n  \"description\": \"Retention schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Number of days to retain metadata\",\n      \"minimum\": 1,\n      \"maximum\": 30,\n      \"example\": 1\n    },\n    \"data\": {\n      \"type\": \"integer\",\n      \"nullable\": true,\n      \"description\": \"Number of days to retain data\",\n      \"minimum\": 0,\n      \"maximum\": 30,\n      \"example\": 1\n    }\n  },\n  \"example\": {\n    \"metadata\": 1,\n    \"data\": 0\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-retention-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: Retention
---
