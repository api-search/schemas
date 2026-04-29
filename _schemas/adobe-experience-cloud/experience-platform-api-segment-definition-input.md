---
description: SegmentDefinitionInput schema
layout: schema
name: SegmentDefinitionInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: expression
  type: object
- description: ''
  name: schema
  type: object
- description: ''
  name: mergePolicyId
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-segment-definition-input-schema.json
slug: experience-platform-api-segment-definition-input
source_filename: experience-platform-api-segment-definition-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-segment-definition-input-schema.json\",\n  \"title\": \"SegmentDefinitionInput\",\n  \"description\": \"SegmentDefinitionInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"expression\",\n    \"schema\",\n    \"mergePolicyId\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"expression\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"PQL\"\n          ]\n        },\n        \"value\": {\n          \"type\": \"string\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"pql/text\",\n           \
  \ \"pql/json\"\n          ]\n        }\n      }\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"mergePolicyId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-segment-definition-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: SegmentDefinitionInput
---
