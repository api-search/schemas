---
description: DisassociateLicenseResponse schema from Amazon Managed Grafana API
layout: schema
name: DisassociateLicenseResponse
properties_list:
- description: ''
  name: workspace
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-disassociate-license-response-schema.json
slug: amazon-managed-grafana-disassociate-license-response
source_filename: amazon-managed-grafana-disassociate-license-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-disassociate-license-response-schema.json\",\n  \"title\": \"DisassociateLicenseResponse\",\n  \"description\": \"DisassociateLicenseResponse schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceDescription\"\n        },\n        {\n          \"description\": \"A structure containing information about the workspace.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"workspace\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-disassociate-license-response-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: DisassociateLicenseResponse
---
