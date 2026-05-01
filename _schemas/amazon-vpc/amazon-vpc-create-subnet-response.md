---
description: Response from the CreateSubnet action
layout: schema
name: CreateSubnetResponse
properties_list:
- description: ''
  name: subnet
  type: object
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-create-subnet-response-schema.json
slug: amazon-vpc-create-subnet-response
source_filename: amazon-vpc-create-subnet-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response from the CreateSubnet action\",\n  \"properties\": {\n    \"subnet\": {\n      \"$ref\": \"#/components/schemas/Subnet\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateSubnetResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-create-subnet-response-schema.json
tags:
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: CreateSubnetResponse
---
