---
description: The parameters for the action type definition that are provided when the action type is created or updated.
layout: schema
name: ActionTypeDeclaration
properties_list:
- description: ''
  name: description
  type: object
- description: ''
  name: executor
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: inputArtifactDetails
  type: object
- description: ''
  name: outputArtifactDetails
  type: object
- description: ''
  name: permissions
  type: object
- description: The properties of the action type to be updated.
  name: properties
  type: object
- description: ''
  name: urls
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-type-declaration-schema.json
slug: amazon-codepipeline-action-type-declaration
source_filename: amazon-codepipeline-action-type-declaration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-declaration-schema.json\",\n  \"title\": \"ActionTypeDeclaration\",\n  \"description\": \"The parameters for the action type definition that are provided when the action type is created or updated.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeDescription\"\n        },\n        {\n          \"description\": \"The description for the action type to be updated.\"\n        }\n      ]\n    },\n    \"executor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeExecutor\"\n        },\n        {\n          \"description\": \"Information about the executor for an action type that was created with any supported integration model.\"\
  \n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeIdentifier\"\n        },\n        {\n          \"description\": \"The action category, owner, provider, and version of the action type to be updated.\"\n        }\n      ]\n    },\n    \"inputArtifactDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeArtifactDetails\"\n        },\n        {\n          \"description\": \"Details for the artifacts, such as application files, to be worked on by the action. For example, the minimum and maximum number of input artifacts allowed.\"\n        }\n      ]\n    },\n    \"outputArtifactDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeArtifactDetails\"\n        },\n        {\n          \"description\": \"Details for the output artifacts, such as a built application, that are the result of the action. For example, the minimum and\
  \ maximum number of output artifacts allowed.\"\n        }\n      ]\n    },\n    \"permissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypePermissions\"\n        },\n        {\n          \"description\": \"Details identifying the accounts with permissions to use the action type.\"\n        }\n      ]\n    },\n    \"properties\": {\n      \"description\": \"The properties of the action type to be updated.\"\n    },\n    \"urls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeUrls\"\n        },\n        {\n          \"description\": \"The links associated with the action type to be updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"executor\",\n    \"id\",\n    \"inputArtifactDetails\",\n    \"outputArtifactDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-declaration-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionTypeDeclaration
---
