---
description: ListFlowsResponse schema from Amazon AppFlow API
layout: schema
name: ListFlowsResponse
properties_list:
- description: The list of flows associated with your account.
  name: flows
  type: array
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-list-flows-response-schema.json
slug: appflow-list-flows-response
source_filename: appflow-list-flows-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-flows-response-schema.json\",\n  \"title\": \"ListFlowsResponse\",\n  \"description\": \"ListFlowsResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flows\": {\n      \"type\": \"array\",\n      \"items\": {},\n      \"description\": \"The list of flows associated with your account.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-flows-response-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ListFlowsResponse
---
