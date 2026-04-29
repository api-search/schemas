---
description: A Bridge is the connection between your datacenter's Instances and the AWS cloud. A bridge can be used to send video from the AWS cloud to your datacenter or from your datacenter to the AWS cloud.
layout: schema
name: Bridge
properties_list:
- description: ''
  name: BridgeArn
  type: object
- description: ''
  name: BridgeMessages
  type: object
- description: ''
  name: BridgeState
  type: object
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
schema_file: json-schema/mediaconnect-api-bridge-schema.json
slug: mediaconnect-api-bridge
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-schema.json\",\n  \"title\": \"Bridge\",\n  \"description\": \"A Bridge is the connection between your datacenter's Instances and the AWS cloud. A bridge can be used to send video from the AWS cloud to your datacenter or from your datacenter to the AWS cloud.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BridgeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeArn\"\n          },\n          \"description\": \"The Amazon Resource Number (ARN) of the bridge.\"\n        }\n      ]\n    },\n    \"BridgeMessages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfMessageDetail\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"bridgeMessages\"\n          }\n        }\n      ]\n    },\n    \"BridgeState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BridgeState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"bridgeState\"\n          }\n        }\n      ]\n    },\n    \"EgressGatewayBridge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EgressGatewayBridge\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"egressGatewayBridge\"\n          }\n        }\n      ]\n    },\n    \"IngressGatewayBridge\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IngressGatewayBridge\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ingressGatewayBridge\"\n          }\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"name\"\n          },\n          \"description\": \"The name of the bridge.\"\n        }\n      ]\n    },\n    \"Outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBridgeOutput\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outputs\"\n          },\n          \"description\": \"The outputs on this bridge.\"\n        }\n      ]\n    },\n    \"PlacementArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"placementArn\"\n          },\n          \"description\": \"The placement Amazon Resource Number (ARN) of the bridge.\"\n        }\n      ]\n    },\n    \"SourceFailoverConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailoverConfig\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceFailoverConfig\"\n          }\n        }\n\
  \      ]\n    },\n    \"Sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfBridgeSource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sources\"\n          },\n          \"description\": \"The sources on this bridge.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BridgeArn\",\n    \"BridgeState\",\n    \"PlacementArn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-bridge-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: Bridge
---
