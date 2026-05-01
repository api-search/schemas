---
description: ModifyVpcEndpointServiceConfigurationRequest schema from Amazon PrivateLink API
layout: schema
name: ModifyVpcEndpointServiceConfigurationRequest
properties_list:
- description: ID of the endpoint service to modify
  name: ServiceId
  type: string
- description: Whether connections require acceptance
  name: AcceptanceRequired
  type: boolean
- description: Private DNS name
  name: PrivateDnsName
  type: string
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-modify-vpc-endpoint-service-configuration-request-schema.json
slug: amazon-privatelink-modify-vpc-endpoint-service-configuration-request
source_filename: amazon-privatelink-modify-vpc-endpoint-service-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-modify-vpc-endpoint-service-configuration-request-schema.json\",\n  \"title\": \"ModifyVpcEndpointServiceConfigurationRequest\",\n  \"description\": \"ModifyVpcEndpointServiceConfigurationRequest schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the endpoint service to modify\"\n    },\n    \"AcceptanceRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether connections require acceptance\"\n    },\n    \"PrivateDnsName\": {\n      \"type\": \"string\",\n      \"description\": \"Private DNS name\"\n    }\n  },\n  \"required\": [\n    \"ServiceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-modify-vpc-endpoint-service-configuration-request-schema.json
tags:
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: ModifyVpcEndpointServiceConfigurationRequest
---
