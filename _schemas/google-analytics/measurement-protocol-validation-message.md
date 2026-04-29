---
description: ValidationMessage schema from Google Analytics API
layout: schema
name: ValidationMessage
properties_list:
- description: Path to the field that caused the validation error.
  name: fieldPath
  type: string
- description: Description of the validation error.
  name: description
  type: string
- description: A code identifying the type of validation error.
  name: validationCode
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/measurement-protocol-validation-message-schema.json
slug: measurement-protocol-validation-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-validation-message-schema.json\",\n  \"title\": \"ValidationMessage\",\n  \"description\": \"ValidationMessage schema from Google Analytics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldPath\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the field that caused the validation error.\",\n      \"example\": \"/example/path\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the validation error.\",\n      \"example\": \"Example description\"\n    },\n    \"validationCode\": {\n      \"type\": \"string\",\n      \"description\": \"A code identifying the type of validation error.\",\n      \"enum\": [\n        \"VALUE_INVALID\",\n        \"VALUE_REQUIRED\",\n        \"NAME_INVALID\",\n        \"\
  NAME_RESERVED\",\n        \"VALUE_OUT_OF_BOUNDS\",\n        \"EXCEEDED_MAX_ENTITIES\",\n        \"NAME_DUPLICATED\"\n      ],\n      \"example\": \"VALUE_INVALID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-validation-message-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: ValidationMessage
---
