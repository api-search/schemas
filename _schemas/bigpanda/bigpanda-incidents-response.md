---
description: List of incidents for an environment.
layout: schema
name: IncidentsResponse
properties_list:
- description: Array of incidents.
  name: incidents
  type: array
provider_name: BigPanda
provider_slug: bigpanda
schema_file: json-schema/bigpanda-incidents-response-schema.json
slug: bigpanda-incidents-response
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"IncidentsResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of incidents for an environment.\",\n  \"properties\": {\n    \"incidents\": {\n      \"type\": \"array\",\n      \"description\": \"Array of incidents.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Incident\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bigpanda/refs/heads/main/json-schema/bigpanda-incidents-response-schema.json
tags:
- Incidents
- Monitoring
- Platform
title: IncidentsResponse
---
