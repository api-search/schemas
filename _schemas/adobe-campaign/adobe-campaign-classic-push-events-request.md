---
description: SOAP envelope containing a batch of real-time events for bulk transactional message processing.
layout: schema
name: PushEventsRequest
properties_list:
- description: Array of rtEvent elements.
  name: events
  type: array
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-push-events-request-schema.json
slug: adobe-campaign-classic-push-events-request
source_filename: adobe-campaign-classic-push-events-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-push-events-request-schema.json\",\n  \"title\": \"PushEventsRequest\",\n  \"description\": \"SOAP envelope containing a batch of real-time events for bulk transactional message processing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Array of rtEvent elements.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/PushEventRequest/properties/rtEvent\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-push-events-request-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: PushEventsRequest
---
