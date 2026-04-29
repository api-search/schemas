---
description: DatasetInput schema
layout: schema
name: DatasetInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: schemaRef
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-dataset-input-schema.json
slug: experience-platform-api-dataset-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-dataset-input-schema.json\",\n  \"title\": \"DatasetInput\",\n  \"description\": \"DatasetInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"schemaRef\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"schemaRef\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"id\",\n        \"contentType\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"contentType\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-dataset-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: DatasetInput
---
