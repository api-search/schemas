---
description: The output of the bridge. A flow output is delivered to the AWS cloud.
layout: schema
name: BridgeFlowOutput
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: FlowSourceArn
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-bridge-flow-output-schema.json
slug: mediaconnect-api-bridge-flow-output
source_filename: mediaconnect-api-bridge-flow-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-flow-output-schema.json\",\n  \"title\": \"BridgeFlowOutput\",\n  \"description\": \"The output of the bridge. A flow output is delivered to the AWS cloud.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The Amazon Resource Number (ARN) of the cloud flow.\"\n        }\n      ]\n    },\n    \"FlowSourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowSourceArn\"\n          },\n          \"description\": \"The Amazon Resource Number\
  \ (ARN) of the flow source.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the bridge's output.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlowSourceArn\",\n    \"FlowArn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-flow-output-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: BridgeFlowOutput
---
