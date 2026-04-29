---
description: Batch schema
layout: schema
name: Batch
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: completed
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-batch-schema.json
slug: experience-platform-api-batch
source_filename: experience-platform-api-batch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-batch-schema.json\",\n  \"title\": \"Batch\",\n  \"description\": \"Batch schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"loading\",\n        \"staging\",\n        \"success\",\n        \"failed\",\n        \"abandoned\"\n      ]\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"completed\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-batch-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Batch
---
