---
description: TransactionalMessageRequest schema
layout: schema
name: TransactionalMessageRequest
properties_list:
- description: Recipient email address.
  name: email
  type: string
- description: Context data for personalizing the transactional message.
  name: ctx
  type: object
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-transactional-message-request-schema.json
slug: campaign-api-transactional-message-request
source_filename: campaign-api-transactional-message-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-transactional-message-request-schema.json\",\n  \"title\": \"TransactionalMessageRequest\",\n  \"description\": \"TransactionalMessageRequest schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"email\",\n    \"ctx\"\n  ],\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Recipient email address.\"\n    },\n    \"ctx\": {\n      \"type\": \"object\",\n      \"description\": \"Context data for personalizing the transactional message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-transactional-message-request-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: TransactionalMessageRequest
---
