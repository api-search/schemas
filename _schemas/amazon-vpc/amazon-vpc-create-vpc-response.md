---
description: Response from the CreateVpc action
layout: schema
name: CreateVpcResponse
properties_list:
- description: ''
  name: vpc
  type: object
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-create-vpc-response-schema.json
slug: amazon-vpc-create-vpc-response
source_filename: amazon-vpc-create-vpc-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response from the CreateVpc action\",\n  \"properties\": {\n    \"vpc\": {\n      \"$ref\": \"#/components/schemas/Vpc\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateVpcResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-create-vpc-response-schema.json
tags:
- AWS
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: CreateVpcResponse
---
