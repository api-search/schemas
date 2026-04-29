---
description: Response from the CreateInternetGateway action
layout: schema
name: CreateInternetGatewayResponse
properties_list:
- description: ''
  name: internetGateway
  type: object
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-create-internet-gateway-response-schema.json
slug: amazon-vpc-create-internet-gateway-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response from the CreateInternetGateway action\",\n  \"properties\": {\n    \"internetGateway\": {\n      \"$ref\": \"#/components/schemas/InternetGateway\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateInternetGatewayResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-create-internet-gateway-response-schema.json
tags:
- AWS
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: CreateInternetGatewayResponse
---
