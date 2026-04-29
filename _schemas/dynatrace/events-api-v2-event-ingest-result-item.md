---
description: The result of ingesting an event for a single entity.
layout: schema
name: EventIngestResultItem
properties_list:
- description: The unique identifier assigned to the created event.
  name: eventId
  type: string
- description: The ingestion status for this entity. OK indicates success; other values indicate warnings or errors.
  name: status
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/events-api-v2-event-ingest-result-item-schema.json
slug: events-api-v2-event-ingest-result-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-event-ingest-result-item-schema.json\",\n  \"title\": \"EventIngestResultItem\",\n  \"description\": \"The result of ingesting an event for a single entity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to the created event.\",\n      \"example\": \"abc123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The ingestion status for this entity. OK indicates success; other values indicate warnings or errors.\",\n      \"example\": \"ACTIVE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-event-ingest-result-item-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: EventIngestResultItem
---
