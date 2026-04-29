---
description: ListConnectorsResponse schema from Amazon AppFlow API
layout: schema
name: ListConnectorsResponse
properties_list:
- description: Contains information about each connector returned in your request.
  name: connectors
  type: array
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-list-connectors-response-schema.json
slug: appflow-list-connectors-response
source_filename: appflow-list-connectors-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-connectors-response-schema.json\",\n  \"title\": \"ListConnectorsResponse\",\n  \"description\": \"ListConnectorsResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectors\": {\n      \"type\": \"array\",\n      \"items\": {},\n      \"description\": \"Contains information about each connector returned in your request.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-connectors-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ListConnectorsResponse
---
