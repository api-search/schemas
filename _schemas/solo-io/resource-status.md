---
description: Status information for a Gloo Gateway resource, indicating whether it has been accepted, rejected, or is pending.
layout: schema
name: Solo.io Gloo Gateway Resource Status
properties_list:
- description: Current state of the resource.
  name: state
  type: string
- description: Reason for the current state.
  name: reason
  type: string
- description: Component that reported this status.
  name: reportedBy
  type: string
provider_name: Solo.io
provider_slug: solo-io
schema_file: json-schema/resource-status.json
slug: resource-status
source_filename: resource-status.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/solo-io/blob/main/json-schema/resource-status.json\",\n  \"title\": \"Solo.io Gloo Gateway Resource Status\",\n  \"description\": \"Status information for a Gloo Gateway resource, indicating whether it has been accepted, rejected, or is pending.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"Pending\", \"Accepted\", \"Rejected\", \"Warning\"],\n      \"description\": \"Current state of the resource.\"\n    },\n    \"reason\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for the current state.\"\n    },\n    \"reportedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Component that reported this status.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/json-schema/resource-status.json
tags:
- AI Gateway
- Analytics
- Automation
- Gateways
- Management
- Monetization
- Observability
- Platform
- Resiliency
- Security
- Service Mesh
- Traffic Control
title: Solo.io Gloo Gateway Resource Status
---
