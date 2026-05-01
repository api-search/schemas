---
description: CancelFlowExecutionsResponse schema from Amazon AppFlow API
layout: schema
name: CancelFlowExecutionsResponse
properties_list:
- description: The IDs of runs that Amazon AppFlow couldn't cancel. The runs might have ended before the cancelation request was processed.
  name: invalidExecutions
  type: array
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-cancel-flow-executions-response-schema.json
slug: appflow-cancel-flow-executions-response
source_filename: appflow-cancel-flow-executions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-cancel-flow-executions-response-schema.json\",\n  \"title\": \"CancelFlowExecutionsResponse\",\n  \"description\": \"CancelFlowExecutionsResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"invalidExecutions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"\"\n      },\n      \"example\": [\n        \"exec-invalid-123\"\n      ],\n      \"description\": \"The IDs of runs that Amazon AppFlow couldn't cancel. The runs might have ended before the cancelation request was processed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-cancel-flow-executions-response-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: CancelFlowExecutionsResponse
---
