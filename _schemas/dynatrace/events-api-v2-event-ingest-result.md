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
schema_file: json-schema/events-api-v2-event-ingest-result-schema.json
slug: events-api-v2-event-ingest-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-event-ingest-result-schema.json\",\n  \"title\": \"EventIngestResult\",\n  \"description\": \"The result returned after successfully ingesting a custom event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of event reports created. This may be greater than 1 if the entitySelector matched multiple entities.\",\n      \"example\": 500\n    },\n    \"eventIngestResults\": {\n      \"type\": \"array\",\n      \"description\": \"Details of each individual event ingestion result.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/EventIngestResultItem\"\n      },\n      \"example\": [\n        {\n          \"eventId\": \"abc123\",\n          \"status\": \"ACTIVE\"\n        }\n      ]\n    }\n  }\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/events-api-v2-event-ingest-result-schema.json
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
