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
schema_file: json-schema/dynatrace-events-v2-event-ingest-result-item-schema.json
slug: dynatrace-events-v2-event-ingest-result-item
source_filename: dynatrace-events-v2-event-ingest-result-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of ingesting an event for a single entity.\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to the created event.\",\n      \"example\": \"abc123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The ingestion status for this entity. OK indicates success; other values indicate warnings or errors.\",\n      \"example\": \"ACTIVE\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventIngestResultItem\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-events-v2-event-ingest-result-item-schema.json
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
