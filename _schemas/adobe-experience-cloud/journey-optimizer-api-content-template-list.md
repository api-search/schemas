---
description: ContentTemplateList schema
layout: schema
name: ContentTemplateList
properties_list:
- description: ''
  name: templates
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/journey-optimizer-api-content-template-list-schema.json
slug: journey-optimizer-api-content-template-list
source_filename: journey-optimizer-api-content-template-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-content-template-list-schema.json\",\n  \"title\": \"ContentTemplateList\",\n  \"description\": \"ContentTemplateList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templates\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"channel\": {\n            \"type\": \"string\"\n          },\n          \"content\": {\n            \"type\": \"object\"\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-content-template-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ContentTemplateList
---
