---
description: Add a flow source to an existing bridge.
layout: schema
name: AddBridgeFlowSourceRequest
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: FlowVpcInterfaceAttachment
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-bridge-flow-source-request-schema.json
slug: mediaconnect-api-add-bridge-flow-source-request
source_filename: mediaconnect-api-add-bridge-flow-source-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-bridge-flow-source-request-schema.json\",\n  \"title\": \"AddBridgeFlowSourceRequest\",\n  \"description\": \"Add a flow source to an existing bridge.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"pattern\": \"^arn:.+:mediaconnect.+:flow:.+$\",\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The Amazon Resource Number (ARN) of the cloud flow to use as a source of this bridge.\"\n        }\n      ]\n    },\n    \"FlowVpcInterfaceAttachment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcInterfaceAttachment\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"flowVpcInterfaceAttachment\"\n          },\n          \"description\": \"The name of the VPC interface attachment to use for this source.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the flow source. This name is used to reference the source and must be unique among sources in this bridge.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlowArn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-bridge-flow-source-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddBridgeFlowSourceRequest
---
