---
description: Information about parameters for artifacts associated with the action type, such as the minimum and maximum artifacts allowed.
layout: schema
name: ActionTypeArtifactDetails
properties_list:
- description: ''
  name: minimumCount
  type: object
- description: ''
  name: maximumCount
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-type-artifact-details-schema.json
slug: amazon-codepipeline-action-type-artifact-details
source_filename: amazon-codepipeline-action-type-artifact-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-artifact-details-schema.json\",\n  \"title\": \"ActionTypeArtifactDetails\",\n  \"description\": \"Information about parameters for artifacts associated with the action type, such as the minimum and maximum artifacts allowed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"minimumCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MinimumActionTypeArtifactCount\"\n        },\n        {\n          \"description\": \"The minimum number of artifacts that can be used with the action type. For example, you should specify a minimum and maximum of zero input artifacts for an action type with a category of <code>source</code>.\"\n        }\n      ]\n    },\n    \"maximumCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/MaximumActionTypeArtifactCount\"\n        },\n        {\n          \"description\": \"The maximum number of artifacts that can be used with the actiontype. For example, you should specify a minimum and maximum of zero input artifacts for an action type with a category of <code>source</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"minimumCount\",\n    \"maximumCount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-type-artifact-details-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionTypeArtifactDetails
---
