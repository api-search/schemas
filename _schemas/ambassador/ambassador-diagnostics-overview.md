---
description: Diagnostic overview of an Ambassador instance
layout: schema
name: DiagnosticsOverview
properties_list:
- description: System-level information
  name: system
  type: object
- description: Active Ambassador configuration summary
  name: ambassador_config
  type: object
- description: Status of the underlying Envoy proxy
  name: envoy_status
  type: object
- description: Summary of active routes
  name: route_info
  type: array
- description: List of configuration errors
  name: errors
  type: array
provider_name: Ambassador
provider_slug: ambassador
schema_file: json-schema/ambassador-diagnostics-overview-schema.json
slug: ambassador-diagnostics-overview
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DiagnosticsOverview\",\n  \"type\": \"object\",\n  \"description\": \"Diagnostic overview of an Ambassador instance\",\n  \"properties\": {\n    \"system\": {\n      \"type\": \"object\",\n      \"description\": \"System-level information\"\n    },\n    \"ambassador_config\": {\n      \"type\": \"object\",\n      \"description\": \"Active Ambassador configuration summary\"\n    },\n    \"envoy_status\": {\n      \"type\": \"object\",\n      \"description\": \"Status of the underlying Envoy proxy\"\n    },\n    \"route_info\": {\n      \"type\": \"array\",\n      \"description\": \"Summary of active routes\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of configuration errors\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ambassador/refs/heads/main/json-schema/ambassador-diagnostics-overview-schema.json
tags:
- API Development
- Gateways
- Ingress
- Kubernetes
- Mock Servers
- Mocks
- Platform
- Testing
title: DiagnosticsOverview
---
