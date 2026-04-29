---
description: Response after ingesting an alert.
layout: schema
name: AlertResponse
properties_list:
- description: Internal alert ID.
  name: _id
  type: string
- description: Ingestion status.
  name: status
  type: string
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-alert-response-schema.json
slug: bigpanda-alert-response
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AlertResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response after ingesting an alert.\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Internal alert ID.\",\n      \"example\": \"alert-abc123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Ingestion status.\",\n      \"example\": \"ok\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-alert-response-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: AlertResponse
---
