---
description: Dataset schema
layout: schema
name: Dataset
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: schemaRef
  type: object
- description: ''
  name: fileDescription
  type: object
- description: ''
  name: created
  type: string
- description: ''
  name: updated
  type: string
- description: ''
  name: status
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-dataset-schema.json
slug: experience-platform-api-dataset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-dataset-schema.json\",\n  \"title\": \"Dataset\",\n  \"description\": \"Dataset schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"schemaRef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"contentType\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"fileDescription\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"format\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"status\": {\n\
  \      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-dataset-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Dataset
---
