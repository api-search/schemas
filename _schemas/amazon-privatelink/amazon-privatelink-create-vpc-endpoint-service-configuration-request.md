---
description: CreateVpcEndpointServiceConfigurationRequest schema from Amazon PrivateLink API
layout: schema
name: CreateVpcEndpointServiceConfigurationRequest
properties_list:
- description: ARNs of Network Load Balancers for the endpoint service
  name: NetworkLoadBalancerArn
  type: array
- description: ARNs of Gateway Load Balancers for the endpoint service
  name: GatewayLoadBalancerArn
  type: array
- description: Whether connection requests require manual acceptance
  name: AcceptanceRequired
  type: boolean
- description: Private DNS name for the endpoint service
  name: PrivateDnsName
  type: string
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-create-vpc-endpoint-service-configuration-request-schema.json
slug: amazon-privatelink-create-vpc-endpoint-service-configuration-request
source_filename: amazon-privatelink-create-vpc-endpoint-service-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-create-vpc-endpoint-service-configuration-request-schema.json\",\n  \"title\": \"CreateVpcEndpointServiceConfigurationRequest\",\n  \"description\": \"CreateVpcEndpointServiceConfigurationRequest schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NetworkLoadBalancerArn\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"ARNs of Network Load Balancers for the endpoint service\"\n    },\n    \"GatewayLoadBalancerArn\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"ARNs of Gateway Load Balancers for the endpoint service\"\n    },\n    \"AcceptanceRequired\": {\n      \"type\": \"boolean\",\n      \"description\"\
  : \"Whether connection requests require manual acceptance\"\n    },\n    \"PrivateDnsName\": {\n      \"type\": \"string\",\n      \"description\": \"Private DNS name for the endpoint service\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-create-vpc-endpoint-service-configuration-request-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: CreateVpcEndpointServiceConfigurationRequest
---
