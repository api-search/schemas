---
description: A request to add VPC interfaces to the flow.
layout: schema
name: AddFlowVpcInterfacesRequest
properties_list:
- description: ''
  name: VpcInterfaces
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-add-flow-vpc-interfaces-request-schema.json
slug: mediaconnect-api-add-flow-vpc-interfaces-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-vpc-interfaces-request-schema.json\",\n  \"title\": \"AddFlowVpcInterfacesRequest\",\n  \"description\": \"A request to add VPC interfaces to the flow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcInterfaces\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfVpcInterfaceRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vpcInterfaces\"\n          },\n          \"description\": \"A list of VPC interfaces that you want to add.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"VpcInterfaces\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-add-flow-vpc-interfaces-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: AddFlowVpcInterfacesRequest
---
