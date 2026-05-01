---
description: Represents the output of a <code>ListActionTypes</code> action.
layout: schema
name: ListActionTypesOutput
properties_list:
- description: ''
  name: actionTypes
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-action-types-output-schema.json
slug: amazon-codepipeline-list-action-types-output
source_filename: amazon-codepipeline-list-action-types-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-action-types-output-schema.json\",\n  \"title\": \"ListActionTypesOutput\",\n  \"description\": \"Represents the output of a <code>ListActionTypes</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeList\"\n        },\n        {\n          \"description\": \"Provides details of the action types.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If the amount of returned information is significantly large, an identifier is also returned. It can be used in a subsequent list action types call to return the next set of\
  \ action types in the list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"actionTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-action-types-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListActionTypesOutput
---
