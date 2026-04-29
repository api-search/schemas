---
description: The source of the bridge. A flow source originates in MediaConnect as an existing cloud flow.
layout: schema
name: BridgeFlowSource
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
- description: ''
  name: OutputArn
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-bridge-flow-source-schema.json
slug: mediaconnect-api-bridge-flow-source
source_filename: mediaconnect-api-bridge-flow-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-flow-source-schema.json\",\n  \"title\": \"BridgeFlowSource\",\n  \"description\": \"The source of the bridge. A flow source originates in MediaConnect as an existing cloud flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the cloud flow used as a source of this bridge.\"\n        }\n      ]\n    },\n    \"FlowVpcInterfaceAttachment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcInterfaceAttachment\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowVpcInterfaceAttachment\"\n\
  \          },\n          \"description\": \"The name of the VPC interface attachment to use for this source.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the flow source.\"\n        }\n      ]\n    },\n    \"OutputArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputArn\"\n          },\n          \"description\": \"The Amazon Resource Number (ARN) of the output.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FlowArn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-flow-source-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: BridgeFlowSource
---
