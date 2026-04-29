---
description: Status information for a Mapping resource
layout: schema
name: MappingStatus
properties_list:
- description: Current state of the Mapping
  name: state
  type: string
- description: Human-readable reason for the current state
  name: reason
  type: string
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-mapping-status-schema.json
slug: ambassador-mapping-status
source_filename: ambassador-mapping-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MappingStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status information for a Mapping resource\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current state of the Mapping\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable reason for the current state\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-mapping-status-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: MappingStatus
---
