---
description: DescribeFlowExecutionRecordsRequest schema from Amazon AppFlow API
layout: schema
name: DescribeFlowExecutionRecordsRequest
properties_list:
- description: The specified name of the flow.
  name: flowName
  type: string
- description: Specifies the maximum number of items that should be returned in the result set.
  name: maxResults
  type: integer
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-flow-execution-records-request-schema.json
slug: appflow-describe-flow-execution-records-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-flow-execution-records-request-schema.json\",\n  \"title\": \"DescribeFlowExecutionRecordsRequest\",\n  \"description\": \"DescribeFlowExecutionRecordsRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-to-s3-flow\",\n      \"description\": \"The specified name of the flow.\"\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 100,\n      \"example\": 20,\n      \"description\": \"Specifies the maximum number of items that should be returned in the result set.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"maxLength\": 2048,\n      \"example\": \"\",\n      \"description\"\
  : \"The pagination token for next page of data.\"\n    }\n  },\n  \"required\": [\n    \"flowName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-flow-execution-records-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeFlowExecutionRecordsRequest
---
