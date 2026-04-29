---
description: TransactionalEventResponse from Adobe Campaign API
layout: schema
name: TransactionalEventResponse
properties_list:
- description: The PKEY of the created event.
  name: PKey
  type: string
- description: Unique identifier of the event.
  name: eventId
  type: string
- description: Initial status of the event.
  name: status
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-transactional-event-response-schema.json
slug: adobe-campaign-standard-transactional-event-response
source_filename: adobe-campaign-standard-transactional-event-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-transactional-event-response-schema.json\",\n  \"title\": \"TransactionalEventResponse\",\n  \"description\": \"TransactionalEventResponse from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\",\n      \"description\": \"The PKEY of the created event.\",\n      \"example\": \"example_value\"\n    },\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the event.\",\n      \"example\": \"CAM123456\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\"\n      ],\n      \"description\": \"Initial status of the event.\",\n      \"example\": \"pending\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-transactional-event-response-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: TransactionalEventResponse
---
