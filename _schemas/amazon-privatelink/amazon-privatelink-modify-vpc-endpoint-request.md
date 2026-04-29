---
description: ModifyVpcEndpointRequest schema from Amazon PrivateLink API
layout: schema
name: ModifyVpcEndpointRequest
properties_list:
- description: ID of the endpoint to modify
  name: VpcEndpointId
  type: string
- description: Reset the policy to the default
  name: ResetPolicy
  type: boolean
- description: New policy document
  name: PolicyDocument
  type: string
provider_name: Amazon PrivateLink
provider_slug: amazon-privatelink
schema_file: json-schema/amazon-privatelink-modify-vpc-endpoint-request-schema.json
slug: amazon-privatelink-modify-vpc-endpoint-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-modify-vpc-endpoint-request-schema.json\",\n  \"title\": \"ModifyVpcEndpointRequest\",\n  \"description\": \"ModifyVpcEndpointRequest schema from Amazon PrivateLink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcEndpointId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the endpoint to modify\"\n    },\n    \"ResetPolicy\": {\n      \"type\": \"boolean\",\n      \"description\": \"Reset the policy to the default\"\n    },\n    \"PolicyDocument\": {\n      \"type\": \"string\",\n      \"description\": \"New policy document\"\n    }\n  },\n  \"required\": [\n    \"VpcEndpointId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-privatelink/refs/heads/main/json-schema/amazon-privatelink-modify-vpc-endpoint-request-schema.json
tags:
- AWS
- Networking
- Private Connectivity
- Security
- VPC
- Zero Trust
- Endpoint Services
title: ModifyVpcEndpointRequest
---
