---
description: ModifyVpcEndpointServicePermissionsRequest schema from Amazon PrivateLink API
layout: schema
name: ModifyVpcEndpointServicePermissionsRequest
properties_list:
- description: ID of the endpoint service
  name: ServiceId
  type: string
- description: Principal ARNs to allow
  name: AddAllowedPrincipals
  type: array
- description: Principal ARNs to remove
  name: RemoveAllowedPrincipals
  type: array
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-modify-vpc-endpoint-service-permissions-request-schema.json
slug: amazon-privatelink-modify-vpc-endpoint-service-permissions-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-modify-vpc-endpoint-service-permissions-request-schema.json\",\n  \"title\": \"ModifyVpcEndpointServicePermissionsRequest\",\n  \"description\": \"ModifyVpcEndpointServicePermissionsRequest schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ServiceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the endpoint service\"\n    },\n    \"AddAllowedPrincipals\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Principal ARNs to allow\"\n    },\n    \"RemoveAllowedPrincipals\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Principal ARNs to remove\"\n    }\n  },\n  \"required\": [\n    \"ServiceId\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-modify-vpc-endpoint-service-permissions-request-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: ModifyVpcEndpointServicePermissionsRequest
---
