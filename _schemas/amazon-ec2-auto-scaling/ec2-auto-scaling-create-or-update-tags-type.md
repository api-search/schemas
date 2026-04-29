---
description: CreateOrUpdateTagsType schema from Auto Scaling
layout: schema
name: CreateOrUpdateTagsType
properties_list:
- description: ''
  name: Tags
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-create-or-update-tags-type-schema.json
slug: ec2-auto-scaling-create-or-update-tags-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-create-or-update-tags-type-schema.json\",\n  \"title\": \"CreateOrUpdateTagsType\",\n  \"description\": \"CreateOrUpdateTagsType schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"One or more tags.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-create-or-update-tags-type-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: CreateOrUpdateTagsType
---
