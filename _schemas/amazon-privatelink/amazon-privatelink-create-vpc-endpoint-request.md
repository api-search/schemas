---
description: CreateVpcEndpointRequest schema from Amazon PrivateLink API
layout: schema
name: CreateVpcEndpointRequest
properties_list:
- description: ID of the VPC for the endpoint
  name: VpcId
  type: string
- description: Service name for the endpoint
  name: ServiceName
  type: string
- description: Type of VPC endpoint
  name: VpcEndpointType
  type: string
- description: IDs of subnets for interface endpoints
  name: SubnetId
  type: array
- description: IDs of security groups for interface endpoints
  name: SecurityGroupId
  type: array
- description: Policy document for gateway endpoints
  name: PolicyDocument
  type: string
- description: Enable private DNS for interface endpoints
  name: PrivateDnsEnabled
  type: boolean
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-create-vpc-endpoint-request-schema.json
slug: amazon-privatelink-create-vpc-endpoint-request
source_filename: amazon-privatelink-create-vpc-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-create-vpc-endpoint-request-schema.json\",\n  \"title\": \"CreateVpcEndpointRequest\",\n  \"description\": \"CreateVpcEndpointRequest schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the VPC for the endpoint\"\n    },\n    \"ServiceName\": {\n      \"type\": \"string\",\n      \"description\": \"Service name for the endpoint\"\n    },\n    \"VpcEndpointType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Interface\",\n        \"Gateway\",\n        \"GatewayLoadBalancer\"\n      ],\n      \"description\": \"Type of VPC endpoint\"\n    },\n    \"SubnetId\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"\
  description\": \"IDs of subnets for interface endpoints\"\n    },\n    \"SecurityGroupId\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of security groups for interface endpoints\"\n    },\n    \"PolicyDocument\": {\n      \"type\": \"string\",\n      \"description\": \"Policy document for gateway endpoints\"\n    },\n    \"PrivateDnsEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable private DNS for interface endpoints\"\n    }\n  },\n  \"required\": [\n    \"VpcId\",\n    \"ServiceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-create-vpc-endpoint-request-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: CreateVpcEndpointRequest
---
