---
description: QueryList schema
layout: schema
name: QueryList
properties_list:
- description: ''
  name: queries
  type: array
- description: ''
  name: _page
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/experience-platform-api-query-list-schema.json
slug: experience-platform-api-query-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-query-list-schema.json\",\n  \"title\": \"QueryList\",\n  \"description\": \"QueryList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"dbName\": {\n            \"type\": \"string\"\n          },\n          \"sql\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"SUBMITTED\",\n              \"IN_PROGRESS\",\n              \"SUCCESS\",\n              \"FAILED\"\n            ]\n          },\n\
  \          \"created\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"updated\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"rowCount\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"_page\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"totalCount\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/experience-platform-api-query-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: QueryList
---
