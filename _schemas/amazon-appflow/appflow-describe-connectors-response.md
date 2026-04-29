---
description: DescribeConnectorsResponse schema from Amazon AppFlow API
layout: schema
name: DescribeConnectorsResponse
properties_list:
- description: The configuration that is applied to the connectors used in the flow.
  name: connectorConfigurations
  type: object
- description: Information about the connectors supported in Amazon AppFlow.
  name: connectors
  type: array
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-connectors-response-schema.json
slug: appflow-describe-connectors-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connectors-response-schema.json\",\n  \"title\": \"DescribeConnectorsResponse\",\n  \"description\": \"DescribeConnectorsResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"connectorConfigurations\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"The configuration that is applied to the connectors used in the flow.\"\n    },\n    \"connectors\": {\n      \"type\": \"array\",\n      \"items\": {},\n      \"description\": \"Information about the connectors supported in Amazon AppFlow.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-connectors-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeConnectorsResponse
---
