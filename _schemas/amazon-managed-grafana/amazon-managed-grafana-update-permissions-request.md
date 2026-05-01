---
description: UpdatePermissionsRequest schema from Amazon Managed Grafana API
layout: schema
name: UpdatePermissionsRequest
properties_list:
- description: ''
  name: updateInstructionBatch
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-update-permissions-request-schema.json
slug: amazon-managed-grafana-update-permissions-request
source_filename: amazon-managed-grafana-update-permissions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-permissions-request-schema.json\",\n  \"title\": \"UpdatePermissionsRequest\",\n  \"description\": \"UpdatePermissionsRequest schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"updateInstructionBatch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateInstructionBatch\"\n        },\n        {\n          \"description\": \"An array of structures that contain the permission updates to make.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"updateInstructionBatch\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-permissions-request-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: UpdatePermissionsRequest
---
