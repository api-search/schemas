---
description: ''
layout: schema
name: DatasetCreateRequest
properties_list:
- description: The name for the new dataset.
  name: name
  type: string
- description: The display name for the dataset.
  name: displayName
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: fields
  type: array
- description: ''
  name: tags
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/prismAnalytics-dataset-create-request-schema.json
slug: prismAnalytics-dataset-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatasetCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the new dataset.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the dataset.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"fields\": {\n      \"type\": \"array\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/prismAnalytics-dataset-create-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: DatasetCreateRequest
---
