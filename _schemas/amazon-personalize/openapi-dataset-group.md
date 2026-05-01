---
description: DatasetGroup schema from Amazon Personalize
layout: schema
name: DatasetGroup
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: datasetGroupArn
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: domain
  type: string
- description: ''
  name: creationDateTime
  type: string
provider_name: Amazon Personalize
provider_slug: amazon-personalize
schema_file: json-schema/openapi-dataset-group-schema.json
slug: openapi-dataset-group
source_filename: openapi-dataset-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/json-schema/openapi-dataset-group-schema.json\",\n  \"title\": \"DatasetGroup\",\n  \"description\": \"DatasetGroup schema from Amazon Personalize\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"datasetGroupArn\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"domain\": {\n      \"type\": \"string\"\n    },\n    \"creationDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/json-schema/openapi-dataset-group-schema.json
tags:
- AI
- Customer Experience
- Machine Learning
- ML
- Personalization
- Recommendations
title: DatasetGroup
---
