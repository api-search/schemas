---
description: TransactionalEventStatus from Adobe Campaign API
layout: schema
name: TransactionalEventStatus
properties_list:
- description: The PKEY of the event.
  name: PKey
  type: string
- description: Unique identifier of the event.
  name: eventId
  type: string
- description: Current processing status of the event.
  name: status
  type: string
- description: Failure reason if the event was not processed.
  name: reason
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-transactional-event-status-schema.json
slug: adobe-campaign-standard-transactional-event-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-transactional-event-status-schema.json\",\n  \"title\": \"TransactionalEventStatus\",\n  \"description\": \"TransactionalEventStatus from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\",\n      \"description\": \"The PKEY of the event.\",\n      \"example\": \"example_value\"\n    },\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the event.\",\n      \"example\": \"CAM123456\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"processing\",\n        \"paused\",\n        \"processed\",\n        \"ignored\",\n        \"deliveryFailed\",\n        \"routingFailed\",\n        \"targetingFailed\",\n        \"tooOld\"\n\
  \      ],\n      \"description\": \"Current processing status of the event.\",\n      \"example\": \"pending\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Failure reason if the event was not processed.\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-transactional-event-status-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: TransactionalEventStatus
---
