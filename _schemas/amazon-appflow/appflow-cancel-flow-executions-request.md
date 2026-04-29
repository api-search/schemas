---
description: CancelFlowExecutionsRequest schema from Amazon AppFlow API
layout: schema
name: CancelFlowExecutionsRequest
properties_list:
- description: The name of a flow with active runs that you want to cancel.
  name: flowName
  type: string
- description: The ID of each active run to cancel. If you omit this parameter, your request ends all active runs that belong to the flow.
  name: executionIds
  type: array
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-cancel-flow-executions-request-schema.json
slug: appflow-cancel-flow-executions-request
source_filename: appflow-cancel-flow-executions-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-cancel-flow-executions-request-schema.json\",\n  \"title\": \"CancelFlowExecutionsRequest\",\n  \"description\": \"CancelFlowExecutionsRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-to-s3-flow\",\n      \"description\": \"The name of a flow with active runs that you want to cancel.\"\n    },\n    \"executionIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"\"\n      },\n      \"example\": [\n        \"exec-500123\"\n      ],\n      \"description\": \"The ID of each active run to cancel. If you omit this parameter, your request ends all active runs that belong to the flow.\"\n    }\n\
  \  },\n  \"required\": [\n    \"flowName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-cancel-flow-executions-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: CancelFlowExecutionsRequest
---
