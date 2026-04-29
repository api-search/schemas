---
description: ListPermissionsResponse schema from Amazon Managed Grafana API
layout: schema
name: ListPermissionsResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: permissions
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-list-permissions-response-schema.json
slug: amazon-managed-grafana-list-permissions-response
source_filename: amazon-managed-grafana-list-permissions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-list-permissions-response-schema.json\",\n  \"title\": \"ListPermissionsResponse\",\n  \"description\": \"ListPermissionsResponse schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use in a subsequent <code>ListPermissions</code> operation to return the next set of results.\"\n        }\n      ]\n    },\n    \"permissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PermissionEntryList\"\n        },\n        {\n          \"description\": \"The permissions returned by the operation.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"permissions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-list-permissions-response-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: ListPermissionsResponse
---
