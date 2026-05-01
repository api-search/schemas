---
description: Represents the status of a workspace.
layout: schema
name: WorkspaceStatus
properties_list:
- description: ''
  name: statusCode
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-workspace-status-schema.json
slug: amazon-managed-prometheus-workspace-status
source_filename: amazon-managed-prometheus-workspace-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-workspace-status-schema.json\",\n  \"title\": \"WorkspaceStatus\",\n  \"description\": \"Represents the status of a workspace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceStatusCode\"\n        },\n        {\n          \"description\": \"Status code of this workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"statusCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-workspace-status-schema.json
tags:
- Containers
- Monitoring
- Observability
- Prometheus
title: WorkspaceStatus
---
