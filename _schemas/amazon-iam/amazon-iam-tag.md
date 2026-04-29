---
description: Tag schema from AWS IAM API
layout: schema
name: Tag
properties_list:
- description: The key name for the tag.
  name: Key
  type: string
- description: The value for the tag.
  name: Value
  type: string
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-tag-schema.json
slug: amazon-iam-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Tag schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"type\": \"string\",\n      \"description\": \"The key name for the tag.\",\n      \"minLength\": 1,\n      \"maxLength\": 128\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The value for the tag.\",\n      \"maxLength\": 256\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-tag-schema.json
tags:
- Access Management
- Authentication
- Authorization
- AWS
- Identity
- Security
title: Tag
---
