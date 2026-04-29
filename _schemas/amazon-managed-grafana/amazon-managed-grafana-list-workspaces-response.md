---
description: ListWorkspacesResponse schema from Amazon Managed Grafana API
layout: schema
name: ListWorkspacesResponse
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: workspaces
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-list-workspaces-response-schema.json
slug: amazon-managed-grafana-list-workspaces-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-list-workspaces-response-schema.json\",\n  \"title\": \"ListWorkspacesResponse\",\n  \"description\": \"ListWorkspacesResponse schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use when requesting the next set of workspaces.\"\n        }\n      ]\n    },\n    \"workspaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceList\"\n        },\n        {\n          \"description\": \"An array of structures that contain some information about the workspaces in the account.\"\n        }\n      ]\n    }\n  },\n  \"required\":\
  \ [\n    \"workspaces\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-list-workspaces-response-schema.json
tags:
- AWS
- Dashboards
- Monitoring
- Observability
- Visualization
title: ListWorkspacesResponse
---
