---
description: VpcEndpointConnection schema from Amazon PrivateLink API
layout: schema
name: VpcEndpointConnection
properties_list:
- description: ID of the endpoint service
  name: ServiceId
  type: string
- description: ID of the VPC endpoint
  name: VpcEndpointId
  type: string
- description: AWS account ID of the endpoint owner
  name: VpcEndpointOwner
  type: string
- description: State of the endpoint
  name: VpcEndpointState
  type: string
- description: Time the connection was created
  name: CreationTimestamp
  type: string
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-vpc-endpoint-connection-schema.json
slug: amazon-privatelink-vpc-endpoint-connection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-vpc-endpoint-connection-schema.json\",\n  \"title\": \"VpcEndpointConnection\",\n  \"description\": \"VpcEndpointConnection schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the endpoint service\"\n    },\n    \"VpcEndpointId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the VPC endpoint\"\n    },\n    \"VpcEndpointOwner\": {\n      \"type\": \"string\",\n      \"description\": \"AWS account ID of the endpoint owner\"\n    },\n    \"VpcEndpointState\": {\n      \"type\": \"string\",\n      \"description\": \"State of the endpoint\"\n    },\n    \"CreationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Time the connection was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-vpc-endpoint-connection-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: VpcEndpointConnection
---
