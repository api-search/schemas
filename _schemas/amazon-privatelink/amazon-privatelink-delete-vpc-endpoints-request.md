---
description: DeleteVpcEndpointsRequest schema from Amazon PrivateLink API
layout: schema
name: DeleteVpcEndpointsRequest
properties_list:
- description: IDs of endpoints to delete
  name: VpcEndpointId
  type: array
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-delete-vpc-endpoints-request-schema.json
slug: amazon-privatelink-delete-vpc-endpoints-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-delete-vpc-endpoints-request-schema.json\",\n  \"title\": \"DeleteVpcEndpointsRequest\",\n  \"description\": \"DeleteVpcEndpointsRequest schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointId\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"IDs of endpoints to delete\"\n    }\n  },\n  \"required\": [\n    \"VpcEndpointId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-delete-vpc-endpoints-request-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: DeleteVpcEndpointsRequest
---
