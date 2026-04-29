---
description: EmailList schema
layout: schema
name: EmailList
properties_list:
- description: ''
  name: content
  type: array
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-email-list-schema.json
slug: campaign-api-email-list
source_filename: campaign-api-email-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-email-list-schema.json\",\n  \"title\": \"EmailList\",\n  \"description\": \"EmailList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"PKey\": {\n            \"type\": \"string\"\n          },\n          \"subject\": {\n            \"type\": \"string\"\n          },\n          \"htmlContent\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\"\n          },\n          \"sender\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"email\": {\n                \"type\"\
  : \"string\"\n              }\n            }\n          },\n          \"created\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-email-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: EmailList
---
