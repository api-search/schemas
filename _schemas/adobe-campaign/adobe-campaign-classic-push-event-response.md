---
description: SOAP response containing the assigned event ID for tracking.
layout: schema
name: PushEventResponse
properties_list:
- description: Unique identifier assigned to the ingested event.
  name: eventId
  type: integer
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-push-event-response-schema.json
slug: adobe-campaign-classic-push-event-response
source_filename: adobe-campaign-classic-push-event-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-push-event-response-schema.json\",\n  \"title\": \"PushEventResponse\",\n  \"description\": \"SOAP response containing the assigned event ID for tracking.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier assigned to the ingested event.\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-push-event-response-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: PushEventResponse
---
