---
description: Returns information about the details of an action type.
layout: schema
name: ActionType
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: settings
  type: object
- description: ''
  name: actionConfigurationProperties
  type: object
- description: ''
  name: inputArtifactDetails
  type: object
- description: ''
  name: outputArtifactDetails
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-type-schema.json
slug: amazon-codepipeline-action-type
source_filename: amazon-codepipeline-action-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-schema.json\",\n  \"title\": \"ActionType\",\n  \"description\": \"Returns information about the details of an action type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeId\"\n        },\n        {\n          \"description\": \"Represents information about an action type.\"\n        }\n      ]\n    },\n    \"settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeSettings\"\n        },\n        {\n          \"description\": \"The settings for the action type.\"\n        }\n      ]\n    },\n    \"actionConfigurationProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionConfigurationPropertyList\"\
  \n        },\n        {\n          \"description\": \"The configuration properties for the action type.\"\n        }\n      ]\n    },\n    \"inputArtifactDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactDetails\"\n        },\n        {\n          \"description\": \"The details of the input artifact for the action, such as its commit ID.\"\n        }\n      ]\n    },\n    \"outputArtifactDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactDetails\"\n        },\n        {\n          \"description\": \"The details of the output artifact of the action, such as its commit ID.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"inputArtifactDetails\",\n    \"outputArtifactDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionType
---
