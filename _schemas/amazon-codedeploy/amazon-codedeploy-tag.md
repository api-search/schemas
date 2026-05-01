---
description: Information about a tag.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-tag-schema.json
slug: amazon-codedeploy-tag
source_filename: amazon-codedeploy-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Information about a tag.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Key\"\n        },\n        {\n          \"description\": \"The tag's key.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Value\"\n        },\n        {\n          \"description\": \"The tag's value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-tag-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: Tag
---
