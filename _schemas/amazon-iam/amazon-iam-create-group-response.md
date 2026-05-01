---
description: CreateGroupResponse schema from AWS IAM API
layout: schema
name: CreateGroupResponse
properties_list:
- description: ''
  name: CreateGroupResult
  type: object
provider_name: Amazon IAM
provider_slug: amazon-iam
schema_file: json-schema/amazon-iam-create-group-response-schema.json
slug: amazon-iam-create-group-response
source_filename: amazon-iam-create-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-group-response-schema.json\",\n  \"title\": \"CreateGroupResponse\",\n  \"description\": \"CreateGroupResponse schema from AWS IAM API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreateGroupResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Group\": {\n          \"$ref\": \"#/components/schemas/Group\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam/refs/heads/main/json-schema/amazon-iam-create-group-response-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity
- Security
title: CreateGroupResponse
---
