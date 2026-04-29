---
description: VpcEndpoint schema from Amazon PrivateLink API
layout: schema
name: VpcEndpoint
properties_list:
- description: ID of the VPC endpoint
  name: VpcEndpointId
  type: string
- description: Type of VPC endpoint
  name: VpcEndpointType
  type: string
- description: ID of the VPC
  name: VpcId
  type: string
- description: Name of the service
  name: ServiceName
  type: string
- description: State of the endpoint
  name: State
  type: string
- description: Policy document
  name: PolicyDocument
  type: string
- description: Subnet IDs for interface endpoints
  name: SubnetIds
  type: array
- description: Network interface IDs
  name: NetworkInterfaceIds
  type: array
- description: DNS entries for the endpoint
  name: DnsEntries
  type: array
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-vpc-endpoint-schema.json
slug: amazon-privatelink-vpc-endpoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-vpc-endpoint-schema.json\",\n  \"title\": \"VpcEndpoint\",\n  \"description\": \"VpcEndpoint schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the VPC endpoint\"\n    },\n    \"VpcEndpointType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of VPC endpoint\"\n    },\n    \"VpcId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the VPC\"\n    },\n    \"ServiceName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the service\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PendingAcceptance\",\n        \"Pending\",\n        \"Available\",\n        \"Deleting\",\n        \"Deleted\"\
  ,\n        \"Rejected\",\n        \"Failed\",\n        \"Expired\"\n      ],\n      \"description\": \"State of the endpoint\"\n    },\n    \"PolicyDocument\": {\n      \"type\": \"string\",\n      \"description\": \"Policy document\"\n    },\n    \"SubnetIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Subnet IDs for interface endpoints\"\n    },\n    \"NetworkInterfaceIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Network interface IDs\"\n    },\n    \"DnsEntries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"DnsName\": {\n            \"type\": \"string\"\n          },\n          \"HostedZoneId\": {\n            \"type\": \"string\"\n          }\n        }\n      },\n      \"description\": \"DNS entries for the endpoint\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-vpc-endpoint-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: VpcEndpoint
---
