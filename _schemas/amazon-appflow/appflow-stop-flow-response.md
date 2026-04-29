---
description: StopFlowResponse schema from Amazon AppFlow API
layout: schema
name: StopFlowResponse
properties_list:
- description: The flow's Amazon Resource Name (ARN).
  name: flowArn
  type: string
- description: Indicates the current status of the flow.
  name: flowStatus
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-stop-flow-response-schema.json
slug: appflow-stop-flow-response
source_filename: appflow-stop-flow-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-stop-flow-response-schema.json\",\n  \"title\": \"StopFlowResponse\",\n  \"description\": \"StopFlowResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowArn\": {\n      \"type\": \"string\",\n      \"example\": \"arn:aws:appflow:us-east-1:123456789012:flow/my-salesforce-to-s3-flow\",\n      \"description\": \"The flow's Amazon Resource Name (ARN).\"\n    },\n    \"flowStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Deprecated\",\n        \"Deleted\",\n        \"Draft\",\n        \"Errored\",\n        \"Suspended\"\n      ],\n      \"example\": \"Suspended\",\n      \"description\": \"Indicates the current status of the flow.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-stop-flow-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: StopFlowResponse
---
