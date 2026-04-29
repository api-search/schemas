---
description: Response from the CreateImage action
layout: schema
name: CreateImageResponse
properties_list:
- description: The ID of the new AMI
  name: imageId
  type: string
provider_name: Amazon EC2
provider_slug: amazon-ec2
schema_file: json-schema/ec2-openapi-create-image-response-schema.json
slug: ec2-openapi-create-image-response
source_filename: ec2-openapi-create-image-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-create-image-response-schema.json\",\n  \"title\": \"CreateImageResponse\",\n  \"description\": \"Response from the CreateImage action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the new AMI\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-create-image-response-schema.json
tags:
- AWS
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
title: CreateImageResponse
---
