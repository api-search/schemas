---
description: Represents the input of a <code>ListActionTypes</code> action.
layout: schema
name: ListActionTypesInput
properties_list:
- description: ''
  name: actionOwnerFilter
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: regionFilter
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-action-types-input-schema.json
slug: amazon-codepipeline-list-action-types-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-action-types-input-schema.json\",\n  \"title\": \"ListActionTypesInput\",\n  \"description\": \"Represents the input of a <code>ListActionTypes</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionOwnerFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionOwner\"\n        },\n        {\n          \"description\": \"Filters the list of action types to those created by a specified entity.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"An identifier that was returned from the previous list action types call, which can be used to return the next set of action types in the list.\"\
  \n        }\n      ]\n    },\n    \"regionFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSRegionName\"\n        },\n        {\n          \"description\": \"The Region to filter on for the list of action types.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-action-types-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListActionTypesInput
---
