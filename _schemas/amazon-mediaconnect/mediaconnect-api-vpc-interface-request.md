---
description: Desired VPC Interface for a Flow
layout: schema
name: VpcInterfaceRequest
properties_list:
- description: ''
  name: Name
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
schema_file: json-schema/mediaconnect-api-vpc-interface-request-schema.json
slug: mediaconnect-api-vpc-interface-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-vpc-interface-request-schema.json\",\n  \"title\": \"VpcInterfaceRequest\",\n  \"description\": \"Desired VPC Interface for a Flow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"The name of the VPC Interface. This value must be unique within the current flow.\"\n        }\n      ]\n    },\n    \"NetworkInterfaceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NetworkInterfaceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkInterfaceType\"\n          },\n          \"description\": \"The type\
  \ of network interface. If this value is not included in the request, MediaConnect uses ENA as the networkInterfaceType.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"roleArn\"\n          },\n          \"description\": \"Role Arn MediaConnect can assumes to create ENIs in customer's account\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroupIds\"\n          },\n          \"description\": \"Security Group IDs to be used on ENI.\"\n        }\n      ]\n    },\n    \"SubnetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetId\"\n    \
  \      },\n          \"description\": \"Subnet must be in the AZ of the Flow\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SubnetId\",\n    \"SecurityGroupIds\",\n    \"RoleArn\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-vpc-interface-request-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: VpcInterfaceRequest
---
