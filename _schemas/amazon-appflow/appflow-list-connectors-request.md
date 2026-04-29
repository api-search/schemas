---
description: ListConnectorsRequest schema from Amazon AppFlow API
layout: schema
name: ListConnectorsRequest
properties_list:
- description: Specifies the maximum number of items that should be returned in the result set.
  name: maxResults
  type: integer
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-list-connectors-request-schema.json
slug: appflow-list-connectors-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-connectors-request-schema.json\",\n  \"title\": \"ListConnectorsRequest\",\n  \"description\": \"ListConnectorsRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 100,\n      \"example\": 20,\n      \"description\": \"Specifies the maximum number of items that should be returned in the result set.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-list-connectors-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ListConnectorsRequest
---
