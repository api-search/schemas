---
description: A revision for an Lambda deployment that is a YAML-formatted or JSON-formatted string. For Lambda deployments, the revision is the same as the AppSpec file.RawString and String revision type are deprecated, use AppSpecContent type instead.
layout: schema
name: RawString
properties_list:
- description: ''
  name: content
  type: object
- description: ''
  name: sha256
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-raw-string-schema.json
slug: amazon-codedeploy-raw-string
source_filename: amazon-codedeploy-raw-string-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-raw-string-schema.json\",\n  \"title\": \"RawString\",\n  \"description\": \"A revision for an Lambda deployment that is a YAML-formatted or JSON-formatted string. For Lambda deployments, the revision is the same as the AppSpec file.RawString and String revision type are deprecated, use AppSpecContent type instead.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RawStringContent\"\n        },\n        {\n          \"description\": \"The YAML-formatted or JSON-formatted revision string. It includes information about which Lambda function to update and optional Lambda functions that validate deployment lifecycle events.\"\n        }\n      ]\n    },\n    \"sha256\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/RawStringSha256\"\n        },\n        {\n          \"description\": \"The SHA256 hash value of the revision content.\"\n        }\n      ]\n    }\n  },\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-raw-string-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: RawString
---
