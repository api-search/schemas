---
description: TransactionalMessageResponse schema
layout: schema
name: TransactionalMessageResponse
properties_list:
- description: ''
  name: PKey
  type: string
- description: ''
  name: eventId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: email
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-transactional-message-response-schema.json
slug: campaign-api-transactional-message-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-transactional-message-response-schema.json\",\n  \"title\": \"TransactionalMessageResponse\",\n  \"description\": \"TransactionalMessageResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\"\n    },\n    \"eventId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"delivered\",\n        \"failed\"\n      ]\n    },\n    \"email\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-transactional-message-response-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: TransactionalMessageResponse
---
