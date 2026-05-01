---
description: TagResourceRequest schema from EC2 Image Builder
layout: schema
name: TagResourceRequest
properties_list:
- description: ''
  name: tags
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-tag-resource-request-schema.json
slug: ec2-image-builder-tag-resource-request
source_filename: ec2-image-builder-tag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-tag-resource-request-schema.json\",\n  \"title\": \"TagResourceRequest\",\n  \"description\": \"TagResourceRequest schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The tags to apply to the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-tag-resource-request-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: TagResourceRequest
---
