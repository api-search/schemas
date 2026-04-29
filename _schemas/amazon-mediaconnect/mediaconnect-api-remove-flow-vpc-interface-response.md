---
description: RemoveFlowVpcInterfaceResponse schema from AWS Elemental MediaConnect API
layout: schema
name: RemoveFlowVpcInterfaceResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: NonDeletedNetworkInterfaceIds
  type: object
- description: ''
  name: VpcInterfaceName
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-remove-flow-vpc-interface-response-schema.json
slug: mediaconnect-api-remove-flow-vpc-interface-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-flow-vpc-interface-response-schema.json\",\n  \"title\": \"RemoveFlowVpcInterfaceResponse\",\n  \"description\": \"RemoveFlowVpcInterfaceResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow that is associated with the VPC interface you removed.\"\n        }\n      ]\n    },\n    \"NonDeletedNetworkInterfaceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nonDeletedNetworkInterfaceIds\"\
  \n          },\n          \"description\": \"IDs of network interfaces associated with the removed VPC interface that Media Connect was unable to remove.\"\n        }\n      ]\n    },\n    \"VpcInterfaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaceName\"\n          },\n          \"description\": \"The name of the VPC interface that was removed.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-remove-flow-vpc-interface-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: RemoveFlowVpcInterfaceResponse
---
