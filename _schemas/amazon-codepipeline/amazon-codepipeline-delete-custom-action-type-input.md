---
description: Represents the input of a <code>DeleteCustomActionType</code> operation. The custom action will be marked as deleted.
layout: schema
name: DeleteCustomActionTypeInput
properties_list:
- description: ''
  name: category
  type: object
- description: ''
  name: provider
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-delete-custom-action-type-input-schema.json
slug: amazon-codepipeline-delete-custom-action-type-input
source_filename: amazon-codepipeline-delete-custom-action-type-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-delete-custom-action-type-input-schema.json\",\n  \"title\": \"DeleteCustomActionTypeInput\",\n  \"description\": \"Represents the input of a <code>DeleteCustomActionType</code> operation. The custom action will be marked as deleted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionCategory\"\n        },\n        {\n          \"description\": \"The category of the custom action that you want to delete, such as source or deploy.\"\n        }\n      ]\n    },\n    \"provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionProvider\"\n        },\n        {\n          \"description\": \"The provider of the service used in the custom action, such\
  \ as CodeDeploy.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the custom action to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"provider\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-delete-custom-action-type-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: DeleteCustomActionTypeInput
---
