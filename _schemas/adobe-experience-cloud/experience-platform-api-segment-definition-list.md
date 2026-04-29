---
description: SegmentDefinitionList schema
layout: schema
name: SegmentDefinitionList
properties_list:
- description: ''
  name: segments
  type: array
- description: ''
  name: page
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-segment-definition-list-schema.json
slug: experience-platform-api-segment-definition-list
source_filename: experience-platform-api-segment-definition-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-segment-definition-list-schema.json\",\n  \"title\": \"SegmentDefinitionList\",\n  \"description\": \"SegmentDefinitionList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"segments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"expression\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"type\": \"string\"\n           \
  \   }\n            }\n          },\n          \"mergePolicyId\": {\n            \"type\": \"string\"\n          },\n          \"evaluationInfo\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"page\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"totalCount\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-segment-definition-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: SegmentDefinitionList
---
