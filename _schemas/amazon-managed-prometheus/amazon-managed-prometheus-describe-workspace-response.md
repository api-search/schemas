---
description: Represents the output of a DescribeWorkspace operation.
layout: schema
name: DescribeWorkspaceResponse
properties_list:
- description: ''
  name: workspace
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-describe-workspace-response-schema.json
slug: amazon-managed-prometheus-describe-workspace-response
source_filename: amazon-managed-prometheus-describe-workspace-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-describe-workspace-response-schema.json\",\n  \"title\": \"DescribeWorkspaceResponse\",\n  \"description\": \"Represents the output of a DescribeWorkspace operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceDescription\"\n        },\n        {\n          \"description\": \"The properties of the selected workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"workspace\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-describe-workspace-response-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: DescribeWorkspaceResponse
---
