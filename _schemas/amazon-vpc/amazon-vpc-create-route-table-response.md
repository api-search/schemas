---
description: Response from the CreateRouteTable action
layout: schema
name: CreateRouteTableResponse
properties_list:
- description: ''
  name: routeTable
  type: object
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-create-route-table-response-schema.json
slug: amazon-vpc-create-route-table-response
source_filename: amazon-vpc-create-route-table-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response from the CreateRouteTable action\",\n  \"properties\": {\n    \"routeTable\": {\n      \"$ref\": \"#/components/schemas/RouteTable\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"CreateRouteTableResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-create-route-table-response-schema.json
tags:
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: CreateRouteTableResponse
---
