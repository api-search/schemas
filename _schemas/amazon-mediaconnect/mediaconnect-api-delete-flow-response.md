---
description: DeleteFlowResponse schema from AWS Elemental MediaConnect API
layout: schema
name: DeleteFlowResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-delete-flow-response-schema.json
slug: mediaconnect-api-delete-flow-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-delete-flow-response-schema.json\",\n  \"title\": \"DeleteFlowResponse\",\n  \"description\": \"DeleteFlowResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow that was deleted.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The status of the flow when the DeleteFlow process begins.\"\n\
  \        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-delete-flow-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: DeleteFlowResponse
---
