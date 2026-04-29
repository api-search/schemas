---
description: Represents the input of a CreateCustomActionType operation.
layout: schema
name: CreateCustomActionTypeInput
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
- description: ''
  name: settings
  type: object
- description: ''
  name: configurationProperties
  type: object
- description: ''
  name: inputArtifactDetails
  type: object
- description: ''
  name: outputArtifactDetails
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-create-custom-action-type-input-schema.json
slug: amazon-codepipeline-create-custom-action-type-input
source_filename: amazon-codepipeline-create-custom-action-type-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-create-custom-action-type-input-schema.json\",\n  \"title\": \"CreateCustomActionTypeInput\",\n  \"description\": \"Represents the input of a CreateCustomActionType operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionCategory\"\n        },\n        {\n          \"description\": \"The category of the custom action, such as a build action or a test action.\"\n        }\n      ]\n    },\n    \"provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionProvider\"\n        },\n        {\n          \"description\": \"The provider of the service used in the custom action, such as CodeDeploy.\"\n        }\n      ]\n    },\n    \"version\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version identifier of the custom action.\"\n        }\n      ]\n    },\n    \"settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeSettings\"\n        },\n        {\n          \"description\": \"URLs that provide users information about this custom action.\"\n        }\n      ]\n    },\n    \"configurationProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionConfigurationPropertyList\"\n        },\n        {\n          \"description\": \"<p>The configuration properties for the custom action.</p> <note> <p>You can refer to a name in the configuration properties of the custom action within the URL templates by following the format of {Config:name}, as long as the configuration property is both required and not secret. For more information, see <a href=\\\"https://docs.aws.amazon.com/codepipeline/latest/userguide/how-to-create-custom-action.html\\\
  \">Create a Custom Action for a Pipeline</a>.</p> </note>\"\n        }\n      ]\n    },\n    \"inputArtifactDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactDetails\"\n        },\n        {\n          \"description\": \"The details of the input artifact for the action, such as its commit ID.\"\n        }\n      ]\n    },\n    \"outputArtifactDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactDetails\"\n        },\n        {\n          \"description\": \"The details of the output artifact of the action, such as its commit ID.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags for the custom action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"provider\",\n    \"version\",\n    \"inputArtifactDetails\",\n    \"outputArtifactDetails\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-create-custom-action-type-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: CreateCustomActionTypeInput
---
