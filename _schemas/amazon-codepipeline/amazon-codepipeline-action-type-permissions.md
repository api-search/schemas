---
description: Details identifying the users with permissions to use the action type.
layout: schema
name: ActionTypePermissions
properties_list:
- description: ''
  name: allowedAccounts
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-type-permissions-schema.json
slug: amazon-codepipeline-action-type-permissions
source_filename: amazon-codepipeline-action-type-permissions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-permissions-schema.json\",\n  \"title\": \"ActionTypePermissions\",\n  \"description\": \"Details identifying the users with permissions to use the action type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowedAccounts\"\n        },\n        {\n          \"description\": \"A list of Amazon Web Services account IDs with access to use the action type in their pipelines.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"allowedAccounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-permissions-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionTypePermissions
---
