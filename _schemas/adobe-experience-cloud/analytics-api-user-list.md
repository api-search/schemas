---
description: UserList schema
layout: schema
name: UserList
properties_list:
- description: ''
  name: content
  type: array
- description: ''
  name: totalElements
  type: integer
- description: ''
  name: totalPages
  type: integer
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/analytics-api-user-list-schema.json
slug: analytics-api-user-list
source_filename: analytics-api-user-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-user-list-schema.json\",\n  \"title\": \"UserList\",\n  \"description\": \"UserList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"loginId\": {\n            \"type\": \"string\"\n          },\n          \"email\": {\n            \"type\": \"string\"\n          },\n          \"firstName\": {\n            \"type\": \"string\"\n          },\n          \"lastName\": {\n            \"type\": \"string\"\n          },\n          \"admin\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    },\n    \"totalElements\": {\n      \"type\": \"integer\"\n  \
  \  },\n    \"totalPages\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/analytics-api-user-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: UserList
---
