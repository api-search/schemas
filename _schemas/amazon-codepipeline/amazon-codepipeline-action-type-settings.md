---
description: Returns information about the settings for an action type.
layout: schema
name: ActionTypeSettings
properties_list:
- description: ''
  name: thirdPartyConfigurationUrl
  type: object
- description: ''
  name: entityUrlTemplate
  type: object
- description: ''
  name: executionUrlTemplate
  type: object
- description: ''
  name: revisionUrlTemplate
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-type-settings-schema.json
slug: amazon-codepipeline-action-type-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-settings-schema.json\",\n  \"title\": \"ActionTypeSettings\",\n  \"description\": \"Returns information about the settings for an action type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"thirdPartyConfigurationUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The URL of a sign-up page where users can sign up for an external service and perform initial configuration of the action provided by that service.\"\n        }\n      ]\n    },\n    \"entityUrlTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UrlTemplate\"\n        },\n        {\n          \"description\": \"The URL returned to the CodePipeline console that provides a deep\
  \ link to the resources of the external system, such as the configuration page for a CodeDeploy deployment group. This link is provided as part of the action display in the pipeline.\"\n        }\n      ]\n    },\n    \"executionUrlTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UrlTemplate\"\n        },\n        {\n          \"description\": \"The URL returned to the CodePipeline console that contains a link to the top-level landing page for the external system, such as the console page for CodeDeploy. This link is shown on the pipeline view page in the CodePipeline console and provides a link to the execution entity of the external action.\"\n        }\n      ]\n    },\n    \"revisionUrlTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UrlTemplate\"\n        },\n        {\n          \"description\": \"The URL returned to the CodePipeline console that contains a link to the page where customers can update\
  \ or change the configuration of the external action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-settings-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionTypeSettings
---
