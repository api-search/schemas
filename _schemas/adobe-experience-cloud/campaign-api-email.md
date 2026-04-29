---
description: Email schema
layout: schema
name: Email
properties_list:
- description: ''
  name: PKey
  type: string
- description: ''
  name: subject
  type: string
- description: ''
  name: htmlContent
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: sender
  type: object
- description: ''
  name: created
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-email-schema.json
slug: campaign-api-email
source_filename: campaign-api-email-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-email-schema.json\",\n  \"title\": \"Email\",\n  \"description\": \"Email schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\"\n    },\n    \"subject\": {\n      \"type\": \"string\"\n    },\n    \"htmlContent\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"sender\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"email\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-email-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Email
---
