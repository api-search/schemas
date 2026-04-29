---
description: AddFlowVpcInterfacesResponse schema from AWS Elemental MediaConnect API
layout: schema
name: AddFlowVpcInterfacesResponse
properties_list:
- description: ''
  name: FlowArn
  type: object
- description: ''
  name: VpcInterfaces
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-flow-vpc-interfaces-response-schema.json
slug: mediaconnect-api-add-flow-vpc-interfaces-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-vpc-interfaces-response-schema.json\",\n  \"title\": \"AddFlowVpcInterfacesResponse\",\n  \"description\": \"AddFlowVpcInterfacesResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flowArn\"\n          },\n          \"description\": \"The ARN of the flow that these VPC interfaces were added to.\"\n        }\n      ]\n    },\n    \"VpcInterfaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfVpcInterface\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaces\"\n          },\n      \
  \    \"description\": \"The details of the newly added VPC interfaces.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-vpc-interfaces-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddFlowVpcInterfacesResponse
---
