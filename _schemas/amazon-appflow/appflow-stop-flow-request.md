---
description: StopFlowRequest schema from Amazon AppFlow API
layout: schema
name: StopFlowRequest
properties_list:
- description: The specified name of the flow.
  name: flowName
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-stop-flow-request-schema.json
slug: appflow-stop-flow-request
source_filename: appflow-stop-flow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-stop-flow-request-schema.json\",\n  \"title\": \"StopFlowRequest\",\n  \"description\": \"StopFlowRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-to-s3-flow\",\n      \"description\": \"The specified name of the flow.\"\n    }\n  },\n  \"required\": [\n    \"flowName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-stop-flow-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: StopFlowRequest
---
