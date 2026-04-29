---
description: Service schema
layout: schema
name: Service
properties_list:
- description: ''
  name: PKey
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: mode
  type: string
- description: ''
  name: created
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-service-schema.json
slug: campaign-api-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"Service schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"label\": {\n      \"type\": \"string\"\n    },\n    \"mode\": {\n      \"type\": \"string\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-service-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Service
---
