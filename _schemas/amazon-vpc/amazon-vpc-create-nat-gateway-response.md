---
description: Response from the CreateNatGateway action
layout: schema
name: CreateNatGatewayResponse
properties_list:
- description: ''
  name: natGateway
  type: object
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-create-nat-gateway-response-schema.json
slug: amazon-vpc-create-nat-gateway-response
source_filename: amazon-vpc-create-nat-gateway-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response from the CreateNatGateway action\",\n  \"properties\": {\n    \"natGateway\": {\n      \"$ref\": \"#/components/schemas/NatGateway\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateNatGatewayResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-create-nat-gateway-response-schema.json
tags:
- AWS
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: CreateNatGatewayResponse
---
