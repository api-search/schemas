---
description: StartFlowResponse schema from Amazon AppFlow API
layout: schema
name: StartFlowResponse
properties_list:
- description: The flow's Amazon Resource Name (ARN).
  name: flowArn
  type: string
- description: Indicates the current status of the flow.
  name: flowStatus
  type: string
- description: Returns the internal execution ID of an on-demand flow when the flow is started.
  name: executionId
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-start-flow-response-schema.json
slug: appflow-start-flow-response
source_filename: appflow-start-flow-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-start-flow-response-schema.json\",\n  \"title\": \"StartFlowResponse\",\n  \"description\": \"StartFlowResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:appflow:us-east-1:123456789012:flow/my-salesforce-to-s3-flow\",\n      \"description\": \"The flow's Amazon Resource Name (ARN).\"\n    },\n    \"flowStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Deprecated\",\n        \"Deleted\",\n        \"Draft\",\n        \"Errored\",\n        \"Suspended\"\n      ],\n      \"example\": \"Active\",\n      \"description\": \"Indicates the current status of the flow.\"\n    },\n    \"executionId\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"exec-500123\",\n      \"description\": \"Returns the internal execution ID of an on-demand flow when the flow is started.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-start-flow-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: StartFlowResponse
---
