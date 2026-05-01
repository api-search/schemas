---
description: Contains information about a batch build build group. Build groups are used to combine builds that can run in parallel, while still being able to set dependencies on other build groups.
layout: schema
name: BuildGroup
properties_list:
- description: ''
  name: identifier
  type: object
- description: ''
  name: dependsOn
  type: object
- description: ''
  name: ignoreFailure
  type: object
- description: ''
  name: currentBuildSummary
  type: object
- description: ''
  name: priorBuildSummaryList
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-group-schema.json
slug: amazon-codebuild-build-group
source_filename: amazon-codebuild-build-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-group-schema.json\",\n  \"title\": \"BuildGroup\",\n  \"description\": \"Contains information about a batch build build group. Build groups are used to combine builds that can run in parallel, while still being able to set dependencies on other build groups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Contains the identifier of the build group.\"\n        }\n      ]\n    },\n    \"dependsOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifiers\"\n        },\n        {\n          \"description\": \"An array of strings that contain the identifiers of the build groups that this build\
  \ group depends on.\"\n        }\n      ]\n    },\n    \"ignoreFailure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specifies if failures in this build group can be ignored.\"\n        }\n      ]\n    },\n    \"currentBuildSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildSummary\"\n        },\n        {\n          \"description\": \"A <code>BuildSummary</code> object that contains a summary of the current build group.\"\n        }\n      ]\n    },\n    \"priorBuildSummaryList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildSummaries\"\n        },\n        {\n          \"description\": \"An array of <code>BuildSummary</code> objects that contain summaries of previous build groups.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-group-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildGroup
---
