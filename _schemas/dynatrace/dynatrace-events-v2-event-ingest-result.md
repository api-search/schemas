---
description: The result returned after successfully ingesting a custom event.
layout: schema
name: EventIngestResult
properties_list:
- description: The number of event reports created. This may be greater than 1 if the entitySelector matched multiple entities.
  name: reportCount
  type: integer
- description: Details of each individual event ingestion result.
  name: eventIngestResults
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-events-v2-event-ingest-result-schema.json
slug: dynatrace-events-v2-event-ingest-result
source_filename: dynatrace-events-v2-event-ingest-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result returned after successfully ingesting a custom event.\",\n  \"properties\": {\n    \"reportCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of event reports created. This may be greater than 1 if the entitySelector matched multiple entities.\",\n      \"example\": 500\n    },\n    \"eventIngestResults\": {\n      \"type\": \"array\",\n      \"description\": \"Details of each individual event ingestion result.\",\n      \"example\": [\n        {\n          \"eventId\": \"abc123\",\n          \"status\": \"ACTIVE\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"The result of ingesting an event for a single entity.\",\n        \"properties\": {\n          \"eventId\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier assigned to the created event.\",\n            \"example\": \"abc123\"\n        \
  \  },\n          \"status\": {\n            \"type\": \"string\",\n            \"description\": \"The ingestion status for this entity. OK indicates success; other values indicate warnings or errors.\",\n            \"example\": \"ACTIVE\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventIngestResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-events-v2-event-ingest-result-schema.json
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
title: EventIngestResult
---
