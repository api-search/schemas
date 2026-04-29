---
description: Response from the ListDashboards action
layout: schema
name: ListDashboardsResponse
properties_list:
- description: The list of matching dashboards
  name: dashboardEntries
  type: array
- description: Token for the next page of results
  name: nextToken
  type: string
provider_name: Amazon CloudWatch
provider_slug: amazon-cloudwatch
schema_file: json-schema/cloudwatch-list-dashboards-response-schema.json
slug: cloudwatch-list-dashboards-response
source_filename: cloudwatch-list-dashboards-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-list-dashboards-response-schema.json\",\n  \"title\": \"ListDashboardsResponse\",\n  \"description\": \"Response from the ListDashboards action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dashboardEntries\": {\n      \"type\": \"array\",\n      \"description\": \"The list of matching dashboards\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Dashboard\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Token for the next page of results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudwatch/refs/heads/main/json-schema/cloudwatch-list-dashboards-response-schema.json
tags:
- AWS
- CloudWatch
- Monitoring
- Observability
- Metrics
- Logs
title: ListDashboardsResponse
---
