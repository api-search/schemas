---
description: Represents information about an action type.
layout: schema
name: ActionTypeId
properties_list:
- description: ''
  name: category
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: provider
  type: object
- description: ''
  name: version
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-type-id-schema.json
slug: amazon-codepipeline-action-type-id
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-id-schema.json\",\n  \"title\": \"ActionTypeId\",\n  \"description\": \"Represents information about an action type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionCategory\"\n        },\n        {\n          \"description\": \"<p>A category defines what kind of action can be taken in the stage, and constrains the provider type for the action. Valid categories are limited to one of the following values. </p> <ul> <li> <p>Source</p> </li> <li> <p>Build</p> </li> <li> <p>Test</p> </li> <li> <p>Deploy</p> </li> <li> <p>Invoke</p> </li> <li> <p>Approval</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"owner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/ActionOwner\"\n        },\n        {\n          \"description\": \"The creator of the action being called. There are three valid values for the <code>Owner</code> field in the action category section within your pipeline structure: <code>AWS</code>, <code>ThirdParty</code>, and <code>Custom</code>. For more information, see <a href=\\\"https://docs.aws.amazon.com/codepipeline/latest/userguide/reference-pipeline-structure.html#actions-valid-providers\\\">Valid Action Types and Providers in CodePipeline</a>.\"\n        }\n      ]\n    },\n    \"provider\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionProvider\"\n        },\n        {\n          \"description\": \"The provider of the service being called by the action. Valid providers are determined by the action category. For example, an action in the Deploy category type might have a provider of CodeDeploy, which would be specified as <code>CodeDeploy</code>. For more information,\
  \ see <a href=\\\"https://docs.aws.amazon.com/codepipeline/latest/userguide/reference-pipeline-structure.html#actions-valid-providers\\\">Valid Action Types and Providers in CodePipeline</a>.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"A string that describes the action version.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"owner\",\n    \"provider\",\n    \"version\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-id-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionTypeId
---
