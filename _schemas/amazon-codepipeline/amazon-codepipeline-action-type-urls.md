---
description: Returns information about URLs for web pages that display to customers as links on the pipeline view, such as an external configuration page for the action type.
layout: schema
name: ActionTypeUrls
properties_list:
- description: ''
  name: configurationUrl
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
schema_file: json-schema/amazon-codepipeline-action-type-urls-schema.json
slug: amazon-codepipeline-action-type-urls
source_filename: amazon-codepipeline-action-type-urls-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-urls-schema.json\",\n  \"title\": \"ActionTypeUrls\",\n  \"description\": \"Returns information about URLs for web pages that display to customers as links on the pipeline view, such as an external configuration page for the action type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The URL returned to the CodePipeline console that contains a link to the page where customers can configure the external action.\"\n        }\n      ]\n    },\n    \"entityUrlTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UrlTemplate\"\n        },\n        {\n          \"description\"\
  : \"The URL returned to the CodePipeline console that provides a deep link to the resources of the external system, such as a status page. This link is provided as part of the action display in the pipeline.\"\n        }\n      ]\n    },\n    \"executionUrlTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UrlTemplate\"\n        },\n        {\n          \"description\": \"The link to an execution page for the action type in progress. For example, for a CodeDeploy action, this link is shown on the pipeline view page in the CodePipeline console, and it links to a CodeDeploy status page.\"\n        }\n      ]\n    },\n    \"revisionUrlTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UrlTemplate\"\n        },\n        {\n          \"description\": \"The URL returned to the CodePipeline console that contains a link to the page where customers can update or change the configuration of the external action.\"\n     \
  \   }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-urls-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionTypeUrls
---
