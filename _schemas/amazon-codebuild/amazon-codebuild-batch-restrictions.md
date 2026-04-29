---
description: Specifies restrictions for the batch build.
layout: schema
name: BatchRestrictions
properties_list:
- description: ''
  name: maximumBuildsAllowed
  type: object
- description: ''
  name: computeTypesAllowed
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-batch-restrictions-schema.json
slug: amazon-codebuild-batch-restrictions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-restrictions-schema.json\",\n  \"title\": \"BatchRestrictions\",\n  \"description\": \"Specifies restrictions for the batch build.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maximumBuildsAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperInt\"\n        },\n        {\n          \"description\": \"Specifies the maximum number of builds allowed.\"\n        }\n      ]\n    },\n    \"computeTypesAllowed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeTypesAllowed\"\n        },\n        {\n          \"description\": \"An array of strings that specify the compute types that are allowed for the batch build. See <a href=\\\"https://docs.aws.amazon.com/codebuild/latest/userguide/build-env-ref-compute-types.html\\\
  \">Build environment compute types</a> in the <i>CodeBuild User Guide</i> for these values. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-batch-restrictions-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BatchRestrictions
---
