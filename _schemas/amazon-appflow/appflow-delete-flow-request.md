---
description: DeleteFlowRequest schema from Amazon AppFlow API
layout: schema
name: DeleteFlowRequest
properties_list:
- description: The specified name of the flow.
  name: flowName
  type: string
- description: Indicates whether Amazon AppFlow should delete the flow, even if it is currently in use.
  name: forceDelete
  type: boolean
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-delete-flow-request-schema.json
slug: appflow-delete-flow-request
source_filename: appflow-delete-flow-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-delete-flow-request-schema.json\",\n  \"title\": \"DeleteFlowRequest\",\n  \"description\": \"DeleteFlowRequest schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"flowName\": {\n      \"type\": \"string\",\n      \"maxLength\": 256,\n      \"example\": \"my-salesforce-to-s3-flow\",\n      \"description\": \"The specified name of the flow.\"\n    },\n    \"forceDelete\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Indicates whether Amazon AppFlow should delete the flow, even if it is currently in use.\"\n    }\n  },\n  \"required\": [\n    \"flowName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-delete-flow-request-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: DeleteFlowRequest
---
