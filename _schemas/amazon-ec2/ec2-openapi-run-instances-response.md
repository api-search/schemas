---
description: Response from the RunInstances action
layout: schema
name: RunInstancesResponse
properties_list:
- description: The ID of the reservation
  name: reservationId
  type: string
- description: The ID of the AWS account that owns the reservation
  name: ownerId
  type: string
- description: The instances launched
  name: instances
  type: array
provider_name: Amazon EC2
provider_slug: amazon-ec2
schema_file: json-schema/ec2-openapi-run-instances-response-schema.json
slug: ec2-openapi-run-instances-response
source_filename: ec2-openapi-run-instances-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-run-instances-response-schema.json\",\n  \"title\": \"RunInstancesResponse\",\n  \"description\": \"Response from the RunInstances action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reservationId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the reservation\"\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the AWS account that owns the reservation\"\n    },\n    \"instances\": {\n      \"type\": \"array\",\n      \"description\": \"The instances launched\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Instance\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-run-instances-response-schema.json
tags:
- AWS
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
title: RunInstancesResponse
---
