---
description: ProfileList schema
layout: schema
name: ProfileList
properties_list:
- description: ''
  name: content
  type: array
- description: ''
  name: count
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-profile-list-schema.json
slug: campaign-api-profile-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-profile-list-schema.json\",\n  \"title\": \"ProfileList\",\n  \"description\": \"ProfileList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"PKey\": {\n            \"type\": \"string\"\n          },\n          \"email\": {\n            \"type\": \"string\"\n          },\n          \"firstName\": {\n            \"type\": \"string\"\n          },\n          \"lastName\": {\n            \"type\": \"string\"\n          },\n          \"birthDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\"\n          },\n          \"phone\": {\n            \"type\": \"string\"\n          },\n          \"created\": {\n            \"\
  type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"lastModified\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"count\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"value\": {\n          \"type\": \"integer\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-profile-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ProfileList
---
