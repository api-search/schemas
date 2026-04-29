---
description: ''
layout: schema
name: EmailNotificationParameters
properties_list:
- description: ''
  name: addresses
  type: array
provider_name: Airbus OneAtlas
provider_slug: airbus-oneatlas
schema_file: json-schema/oneatlas-email-notification-parameters-schema.json
slug: oneatlas-email-notification-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-email-notification-parameters-schema.json\",\n  \"title\": \"EmailNotificationParameters\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addresses\": {\n      \"items\": {\n        \"description\": \"To be done: Email need to be validated.\",\n        \"format\": \"email\",\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"addresses\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbus-oneatlas/refs/heads/main/json-schema/oneatlas-email-notification-parameters-schema.json
tags:
- Imagery
- Satellites
title: EmailNotificationParameters
---
