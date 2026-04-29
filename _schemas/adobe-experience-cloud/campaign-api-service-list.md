---
description: ServiceList schema
layout: schema
name: ServiceList
properties_list:
- description: ''
  name: content
  type: array
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-service-list-schema.json
slug: campaign-api-service-list
source_filename: campaign-api-service-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-service-list-schema.json\",\n  \"title\": \"ServiceList\",\n  \"description\": \"ServiceList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"PKey\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"label\": {\n            \"type\": \"string\"\n          },\n          \"mode\": {\n            \"type\": \"string\"\n          },\n          \"created\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-service-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ServiceList
---
