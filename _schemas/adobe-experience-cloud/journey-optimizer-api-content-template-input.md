---
description: ContentTemplateInput schema
layout: schema
name: ContentTemplateInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: channel
  type: string
- description: ''
  name: content
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/journey-optimizer-api-content-template-input-schema.json
slug: journey-optimizer-api-content-template-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-content-template-input-schema.json\",\n  \"title\": \"ContentTemplateInput\",\n  \"description\": \"ContentTemplateInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"channel\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"email\",\n        \"push\",\n        \"sms\",\n        \"inApp\"\n      ]\n    },\n    \"content\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-content-template-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ContentTemplateInput
---
