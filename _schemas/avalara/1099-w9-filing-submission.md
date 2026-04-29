---
description: FilingSubmission schema from Avalara API
layout: schema
name: FilingSubmission
properties_list:
- description: ''
  name: taxYear
  type: integer
- description: ''
  name: formIds
  type: array
- description: ''
  name: corrected
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/1099-w9-filing-submission-schema.json
slug: 1099-w9-filing-submission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-filing-submission-schema.json\",\n  \"title\": \"FilingSubmission\",\n  \"description\": \"FilingSubmission schema from Avalara API\",\n  \"type\": \"object\",\n  \"required\": [\n    \"taxYear\",\n    \"formIds\"\n  ],\n  \"properties\": {\n    \"taxYear\": {\n      \"type\": \"integer\"\n    },\n    \"formIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"corrected\": {\n      \"type\": \"boolean\",\n      \"default\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-filing-submission-schema.json
tags:
- Taxes
title: FilingSubmission
---
