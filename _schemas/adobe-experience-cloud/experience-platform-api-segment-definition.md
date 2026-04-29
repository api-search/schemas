---
description: SegmentDefinition schema
layout: schema
name: SegmentDefinition
properties_list:
- description: ''
  name: id
  type: string
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
  name: mergePolicyId
  type: string
- description: ''
  name: evaluationInfo
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-segment-definition-schema.json
slug: experience-platform-api-segment-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-segment-definition-schema.json\",\n  \"title\": \"SegmentDefinition\",\n  \"description\": \"SegmentDefinition schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"expression\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\"\n        },\n        \"value\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"mergePolicyId\": {\n      \"type\": \"string\"\n    },\n    \"evaluationInfo\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-segment-definition-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: SegmentDefinition
---
