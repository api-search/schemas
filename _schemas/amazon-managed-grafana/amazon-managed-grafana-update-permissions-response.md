---
description: UpdatePermissionsResponse schema from Amazon Managed Grafana API
layout: schema
name: UpdatePermissionsResponse
properties_list:
- description: ''
  name: errors
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-update-permissions-response-schema.json
slug: amazon-managed-grafana-update-permissions-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-permissions-response-schema.json\",\n  \"title\": \"UpdatePermissionsResponse\",\n  \"description\": \"UpdatePermissionsResponse schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UpdateErrorList\"\n        },\n        {\n          \"description\": \"An array of structures that contain the errors from the operation, if any.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"errors\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-update-permissions-response-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: UpdatePermissionsResponse
---
