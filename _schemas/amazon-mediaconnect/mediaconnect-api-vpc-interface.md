---
description: The settings for a VPC Source.
layout: schema
name: VpcInterface
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: NetworkInterfaceIds
  type: object
- description: ''
  name: NetworkInterfaceType
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
- description: ''
  name: SubnetId
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-vpc-interface-schema.json
slug: mediaconnect-api-vpc-interface
source_filename: mediaconnect-api-vpc-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-vpc-interface-schema.json\",\n  \"title\": \"VpcInterface\",\n  \"description\": \"The settings for a VPC Source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"Immutable and has to be a unique against other VpcInterfaces in this Flow.\"\n        }\n      ]\n    },\n    \"NetworkInterfaceIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkInterfaceIds\"\n          },\n          \"description\": \"IDs of the network interfaces created\
  \ in customer's account by MediaConnect.\"\n        }\n      ]\n    },\n    \"NetworkInterfaceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkInterfaceType\"\n          },\n          \"description\": \"The type of network interface.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"Role Arn MediaConnect can assumes to create ENIs in customer's account\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroupIds\"\n          },\n          \"description\": \"Security Group\
  \ IDs to be used on ENI.\"\n        }\n      ]\n    },\n    \"SubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetId\"\n          },\n          \"description\": \"Subnet must be in the AZ of the Flow\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"NetworkInterfaceType\",\n    \"NetworkInterfaceIds\",\n    \"SubnetId\",\n    \"SecurityGroupIds\",\n    \"RoleArn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-vpc-interface-schema.json
tags:
- Broadcasting
- Live Video
- Media
- Media Transport
title: VpcInterface
---
