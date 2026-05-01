---
description: DescribeConnectorsRequest schema from Amazon AppFlow API
layout: schema
name: DescribeConnectorsRequest
properties_list:
- description: The type of connector, such as Salesforce, Marketo, and so on.
  name: connectorTypes
  type: array
- description: The maximum number of items that should be returned in the result set.
  name: maxResults
  type: integer
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-connectors-request-schema.json
slug: appflow-describe-connectors-request
source_filename: appflow-describe-connectors-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connectors-request-schema.json\",\n  \"title\": \"DescribeConnectorsRequest\",\n  \"description\": \"DescribeConnectorsRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"\"\n      },\n      \"example\": [\n        \"Salesforce\",\n        \"S3\"\n      ],\n      \"description\": \"The type of connector, such as Salesforce, Marketo, and so on.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 100,\n      \"example\": 20,\n      \"description\": \"The maximum number of items that should be returned in the result set.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\
  ,\n      \"maxLength\": 2048,\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connectors-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeConnectorsRequest
---
