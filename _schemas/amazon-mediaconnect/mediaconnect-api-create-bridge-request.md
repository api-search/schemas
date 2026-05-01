---
description: Creates a new bridge. The request must include one source.
layout: schema
name: CreateBridgeRequest
properties_list:
- description: ''
  name: EgressGatewayBridge
  type: object
- description: ''
  name: IngressGatewayBridge
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Outputs
  type: object
- description: ''
  name: PlacementArn
  type: object
- description: ''
  name: SourceFailoverConfig
  type: object
- description: ''
  name: Sources
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-create-bridge-request-schema.json
slug: mediaconnect-api-create-bridge-request
source_filename: mediaconnect-api-create-bridge-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-create-bridge-request-schema.json\",\n  \"title\": \"CreateBridgeRequest\",\n  \"description\": \"Creates a new bridge. The request must include one source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EgressGatewayBridge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddEgressGatewayBridgeRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"egressGatewayBridge\"\n          },\n          \"description\": \"Create a bridge with the egress bridge type. An egress bridge is a cloud-to-ground bridge. The content comes from an existing MediaConnect flow and is delivered to your premises.\"\n        }\n      ]\n    },\n    \"IngressGatewayBridge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddIngressGatewayBridgeRequest\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"ingressGatewayBridge\"\n          },\n          \"description\": \"Create a bridge with the ingress bridge type. An ingress bridge is a ground-to-cloud bridge. The content originates at your premises and is delivered to the cloud.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the bridge. This name can not be modified after the bridge is created.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAddBridgeOutputRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputs\"\n          },\n          \"description\": \"The outputs that you want to add to this bridge.\"\n        }\n      ]\n    },\n\
  \    \"PlacementArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"placementArn\"\n          },\n          \"description\": \"The bridge placement Amazon Resource Number (ARN).\"\n        }\n      ]\n    },\n    \"SourceFailoverConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailoverConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceFailoverConfig\"\n          },\n          \"description\": \"The settings for source failover.\"\n        }\n      ]\n    },\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfAddBridgeSourceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          },\n          \"description\": \"The sources that you want to add to this bridge.\"\n        }\n      ]\n    }\n  },\n  \"required\":\
  \ [\n    \"Sources\",\n    \"PlacementArn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-create-bridge-request-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: CreateBridgeRequest
---
