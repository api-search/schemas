---
description: Represents the output of a ListWorkspaces operation.
layout: schema
name: ListWorkspacesResponse
properties_list:
- description: ''
  name: workspaces
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-list-workspaces-response-schema.json
slug: amazon-managed-prometheus-list-workspaces-response
source_filename: amazon-managed-prometheus-list-workspaces-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-list-workspaces-response-schema.json\",\n  \"title\": \"ListWorkspacesResponse\",\n  \"description\": \"Represents the output of a ListWorkspaces operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workspaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceSummaryList\"\n        },\n        {\n          \"description\": \"The list of existing workspaces, including those undergoing creation or deletion.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"Pagination token to use when requesting the next page in this list.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"workspaces\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-list-workspaces-response-schema.json
tags:
- Containers
- Monitoring
- Observability
- Prometheus
title: ListWorkspacesResponse
---
