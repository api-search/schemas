---
description: Contains configuration information about a batch build project.
layout: schema
name: ProjectBuildBatchConfig
properties_list:
- description: ''
  name: serviceRole
  type: object
- description: ''
  name: combineArtifacts
  type: object
- description: ''
  name: restrictions
  type: object
- description: ''
  name: timeoutInMins
  type: object
- description: ''
  name: batchReportMode
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-project-build-batch-config-schema.json
slug: amazon-codebuild-project-build-batch-config
source_filename: amazon-codebuild-project-build-batch-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-build-batch-config-schema.json\",\n  \"title\": \"ProjectBuildBatchConfig\",\n  \"description\": \"Contains configuration information about a batch build project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Specifies the service role ARN for the batch build project.\"\n        }\n      ]\n    },\n    \"combineArtifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \"Specifies if the build artifacts for the batch build should be combined into a single artifact location.\"\n        }\n      ]\n    },\n    \"\
  restrictions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchRestrictions\"\n        },\n        {\n          \"description\": \"A <code>BatchRestrictions</code> object that specifies the restrictions for the batch build.\"\n        }\n      ]\n    },\n    \"timeoutInMins\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperInt\"\n        },\n        {\n          \"description\": \"Specifies the maximum amount of time, in minutes, that the batch build must be completed in.\"\n        }\n      ]\n    },\n    \"batchReportMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchReportModeType\"\n        },\n        {\n          \"description\": \"<p>Specifies how build status reports are sent to the source provider for the batch build. This property is only used when the source provider for your project is Bitbucket, GitHub, or GitHub Enterprise, and your project is configured to report\
  \ build statuses to the source provider.</p> <dl> <dt>REPORT_AGGREGATED_BATCH</dt> <dd> <p>(Default) Aggregate all of the build statuses into a single status report.</p> </dd> <dt>REPORT_INDIVIDUAL_BUILDS</dt> <dd> <p>Send a separate status report for each individual build.</p> </dd> </dl>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-project-build-batch-config-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ProjectBuildBatchConfig
---
