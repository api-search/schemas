---
description: AcceptVpcEndpointConnectionsRequest schema from Amazon PrivateLink API
layout: schema
name: AcceptVpcEndpointConnectionsRequest
properties_list:
- description: ID of the endpoint service
  name: ServiceId
  type: string
- description: IDs of endpoints to accept
  name: VpcEndpointId
  type: array
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-accept-vpc-endpoint-connections-request-schema.json
slug: amazon-privatelink-accept-vpc-endpoint-connections-request
source_filename: amazon-privatelink-accept-vpc-endpoint-connections-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-accept-vpc-endpoint-connections-request-schema.json\",\n  \"title\": \"AcceptVpcEndpointConnectionsRequest\",\n  \"description\": \"AcceptVpcEndpointConnectionsRequest schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the endpoint service\"\n    },\n    \"VpcEndpointId\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of endpoints to accept\"\n    }\n  },\n  \"required\": [\n    \"ServiceId\",\n    \"VpcEndpointId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-accept-vpc-endpoint-connections-request-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: AcceptVpcEndpointConnectionsRequest
---
