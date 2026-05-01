---
description: ListVersionsResponse schema from Amazon Managed Grafana API
layout: schema
name: ListVersionsResponse
properties_list:
- description: ''
  name: grafanaVersions
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Managed Grafana
provider_slug: amazon-managed-grafana
schema_file: json-schema/amazon-managed-grafana-list-versions-response-schema.json
slug: amazon-managed-grafana-list-versions-response
source_filename: amazon-managed-grafana-list-versions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-list-versions-response-schema.json\",\n  \"title\": \"ListVersionsResponse\",\n  \"description\": \"ListVersionsResponse schema from Amazon Managed Grafana API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grafanaVersions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GrafanaVersionList\"\n        },\n        {\n          \"description\": \"The Grafana versions available to create. If a workspace ID is included in the request, the Grafana versions to which this workspace can be upgraded.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The token to use in a subsequent <code>ListVersions</code>\
  \ operation to return the next set of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-grafana/refs/heads/main/json-schema/amazon-managed-grafana-list-versions-response-schema.json
tags:
- Dashboards
- Monitoring
- Observability
- Visualization
title: ListVersionsResponse
---
