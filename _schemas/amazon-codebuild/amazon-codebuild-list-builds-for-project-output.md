---
description: ListBuildsForProjectOutput schema from Amazon CodeBuild
layout: schema
name: ListBuildsForProjectOutput
properties_list:
- description: ''
  name: ids
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-builds-for-project-output-schema.json
slug: amazon-codebuild-list-builds-for-project-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-builds-for-project-output-schema.json\",\n  \"title\": \"ListBuildsForProjectOutput\",\n  \"description\": \"ListBuildsForProjectOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ids\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildIds\"\n        },\n        {\n          \"description\": \"A list of build identifiers for the specified build project, with each build ID representing a single build.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"If there are more than 100 items in the list, only the first 100 items are returned, along with a unique string called a <i>nextToken</i>.\
  \ To get the next batch of items in the list, call this operation again, adding the next token to the call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-builds-for-project-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListBuildsForProjectOutput
---
