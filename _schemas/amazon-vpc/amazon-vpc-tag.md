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
provider_name: Amazon VPC
provider_slug: amazon-vpc
schema_file: json-schema/amazon-vpc-tag-schema.json
slug: amazon-vpc-tag
source_filename: amazon-vpc-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Describes a tag\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the tag\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the tag\"\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Tag\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-vpc/refs/heads/main/json-schema/amazon-vpc-tag-schema.json
tags:
- Networking
- Private Cloud
- Security
- Subnets
- VPC
title: Tag
---
