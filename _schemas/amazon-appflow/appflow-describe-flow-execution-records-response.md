---
description: DescribeFlowExecutionRecordsResponse schema from Amazon AppFlow API
layout: schema
name: DescribeFlowExecutionRecordsResponse
properties_list:
- description: Returns the execution details and flow run history for a given flow.
  name: flowExecutions
  type: array
- description: The pagination token for next page of data.
  name: nextToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-describe-flow-execution-records-response-schema.json
slug: appflow-describe-flow-execution-records-response
source_filename: appflow-describe-flow-execution-records-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-flow-execution-records-response-schema.json\",\n  \"title\": \"DescribeFlowExecutionRecordsResponse\",\n  \"description\": \"DescribeFlowExecutionRecordsResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowExecutions\": {\n      \"type\": \"array\",\n      \"items\": {},\n      \"description\": \"Returns the execution details and flow run history for a given flow.\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"example\": \"\",\n      \"description\": \"The pagination token for next page of data.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-describe-flow-execution-records-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DescribeFlowExecutionRecordsResponse
---
