---
description: Solution schema from Amazon Personalize
layout: schema
name: Solution
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: solutionArn
  type: string
- description: ''
  name: recipeArn
  type: string
- description: ''
  name: datasetGroupArn
  type: string
- description: ''
  name: status
  type: string
provider_name: Amazon Personalize
provider_slug: amazon-personalize
schema_file: json-schema/openapi-solution-schema.json
slug: openapi-solution
source_filename: openapi-solution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/json-schema/openapi-solution-schema.json\",\n  \"title\": \"Solution\",\n  \"description\": \"Solution schema from Amazon Personalize\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"solutionArn\": {\n      \"type\": \"string\"\n    },\n    \"recipeArn\": {\n      \"type\": \"string\"\n    },\n    \"datasetGroupArn\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/json-schema/openapi-solution-schema.json
tags:
- AI
- AWS
- Customer Experience
- Machine Learning
- ML
- Personalization
- Recommendations
title: Solution
---
