---
description: ListFlowsRequest schema from Amazon AppFlow API
layout: schema
name: ListFlowsRequest
properties_list:
- description: Specifies the maximum number of items that should be returned in the result set.
  name: maxResults
  type: integer
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-list-flows-request-schema.json
slug: appflow-list-flows-request
source_filename: appflow-list-flows-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-flows-request-schema.json\",\n  \"title\": \"ListFlowsRequest\",\n  \"description\": \"ListFlowsRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 100,\n      \"example\": 20,\n      \"description\": \"Specifies the maximum number of items that should be returned in the result set.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"maxLength\": 2048,\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-flows-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ListFlowsRequest
---
