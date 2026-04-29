---
description: UpdateFlowResponse schema from Amazon AppFlow API
layout: schema
name: UpdateFlowResponse
properties_list:
- description: Indicates the current status of the flow.
  name: flowStatus
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-update-flow-response-schema.json
slug: appflow-update-flow-response
source_filename: appflow-update-flow-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-flow-response-schema.json\",\n  \"title\": \"UpdateFlowResponse\",\n  \"description\": \"UpdateFlowResponse schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Active\",\n        \"Deprecated\",\n        \"Deleted\",\n        \"Draft\",\n        \"Errored\",\n        \"Suspended\"\n      ],\n      \"example\": \"Active\",\n      \"description\": \"Indicates the current status of the flow.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-update-flow-response-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: UpdateFlowResponse
---
