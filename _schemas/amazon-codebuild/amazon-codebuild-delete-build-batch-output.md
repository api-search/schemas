---
description: DeleteBuildBatchOutput schema from Amazon CodeBuild
layout: schema
name: DeleteBuildBatchOutput
properties_list:
- description: ''
  name: statusCode
  type: object
- description: ''
  name: buildsDeleted
  type: object
- description: ''
  name: buildsNotDeleted
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-delete-build-batch-output-schema.json
slug: amazon-codebuild-delete-build-batch-output
source_filename: amazon-codebuild-delete-build-batch-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-delete-build-batch-output-schema.json\",\n  \"title\": \"DeleteBuildBatchOutput\",\n  \"description\": \"DeleteBuildBatchOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The status code.\"\n        }\n      ]\n    },\n    \"buildsDeleted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildIds\"\n        },\n        {\n          \"description\": \"An array of strings that contain the identifiers of the builds that were deleted.\"\n        }\n      ]\n    },\n    \"buildsNotDeleted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildsNotDeleted\"\
  \n        },\n        {\n          \"description\": \"An array of <code>BuildNotDeleted</code> objects that specify the builds that could not be deleted.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-delete-build-batch-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: DeleteBuildBatchOutput
---
