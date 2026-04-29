---
description: ActionDeclaration schema from Amazon CodePipeline
layout: schema
name: ActionDeclaration
properties_list:
- description: The action declaration name.
  name: name
  type: string
- description: ''
  name: actionTypeId
  type: object
- description: ''
  name: configuration
  type: object
- description: ''
  name: inputArtifacts
  type: array
- description: ''
  name: outputArtifacts
  type: array
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-declaration-schema.json
slug: amazon-codepipeline-action-declaration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-declaration-schema.json\",\n  \"title\": \"ActionDeclaration\",\n  \"description\": \"ActionDeclaration schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The action declaration name.\"\n    },\n    \"actionTypeId\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"category\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Source\",\n            \"Build\",\n            \"Deploy\",\n            \"Test\",\n            \"Invoke\",\n            \"Approval\"\n          ]\n        },\n        \"owner\": {\n          \"type\": \"string\"\n        },\n        \"provider\": {\n          \"type\": \"string\"\n        },\n        \"version\"\
  : {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"configuration\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"inputArtifacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"outputArtifacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"actionTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-declaration-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionDeclaration
---
