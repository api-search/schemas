---
description: Campaign schema from Amazon Personalize
layout: schema
name: Campaign
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: campaignArn
  type: string
- description: ''
  name: solutionVersionArn
  type: string
- description: ''
  name: minProvisionedTPS
  type: integer
- description: ''
  name: status
  type: string
provider_name: Amazon Personalize
provider_slug: amazon-personalize
schema_file: json-schema/openapi-campaign-schema.json
slug: openapi-campaign
source_filename: openapi-campaign-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/json-schema/openapi-campaign-schema.json\",\n  \"title\": \"Campaign\",\n  \"description\": \"Campaign schema from Amazon Personalize\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"campaignArn\": {\n      \"type\": \"string\"\n    },\n    \"solutionVersionArn\": {\n      \"type\": \"string\"\n    },\n    \"minProvisionedTPS\": {\n      \"type\": \"integer\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-personalize/refs/heads/main/json-schema/openapi-campaign-schema.json
tags:
- AI
- AWS
- Customer Experience
- Machine Learning
- ML
- Personalization
- Recommendations
title: Campaign
---
