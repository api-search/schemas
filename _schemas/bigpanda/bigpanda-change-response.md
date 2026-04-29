---
description: Response after ingesting a change event.
layout: schema
name: ChangeResponse
properties_list:
- description: Internal change ID.
  name: _id
  type: string
- description: Ingestion status.
  name: status
  type: string
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-change-response-schema.json
slug: bigpanda-change-response
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ChangeResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response after ingesting a change event.\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Internal change ID.\",\n      \"example\": \"chg-abc123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Ingestion status.\",\n      \"example\": \"ok\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-change-response-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: ChangeResponse
---
