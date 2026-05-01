---
description: Describes a tag
layout: schema
name: Tag
properties_list:
- description: The key of the tag
  name: key
  type: string
- description: The value of the tag
  name: value
  type: string
provider_name: Amazon EC2
provider_slug: amazon-ec2
schema_file: json-schema/ec2-openapi-tag-schema.json
slug: ec2-openapi-tag
source_filename: ec2-openapi-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Describes a tag\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the tag\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the tag\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2/refs/heads/main/json-schema/ec2-openapi-tag-schema.json
tags:
- Cloud Computing
- Compute
- IaaS
- Infrastructure
- Virtual Machines
title: Tag
---
