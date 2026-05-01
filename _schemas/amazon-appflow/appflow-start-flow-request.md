---
description: StartFlowRequest schema from Amazon AppFlow API
layout: schema
name: StartFlowRequest
properties_list:
- description: The specified name of the flow.
  name: flowName
  type: string
- description: Idempotency token.
  name: clientToken
  type: string
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-start-flow-request-schema.json
slug: appflow-start-flow-request
source_filename: appflow-start-flow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-start-flow-request-schema.json\",\n  \"title\": \"StartFlowRequest\",\n  \"description\": \"StartFlowRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-to-s3-flow\",\n      \"description\": \"The specified name of the flow.\"\n    },\n    \"clientToken\": {\n      \"type\": \"string\",\n      \"example\": \"client-token-500123\",\n      \"description\": \"Idempotency token.\"\n    }\n  },\n  \"required\": [\n    \"flowName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-start-flow-request-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: StartFlowRequest
---
