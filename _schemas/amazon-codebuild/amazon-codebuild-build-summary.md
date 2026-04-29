---
description: Contains summary information about a batch build group.
layout: schema
name: BuildSummary
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: requestedOn
  type: object
- description: ''
  name: buildStatus
  type: object
- description: ''
  name: primaryArtifact
  type: object
- description: ''
  name: secondaryArtifacts
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-summary-schema.json
slug: amazon-codebuild-build-summary
source_filename: amazon-codebuild-build-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-summary-schema.json\",\n  \"title\": \"BuildSummary\",\n  \"description\": \"Contains summary information about a batch build group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The batch build ARN.\"\n        }\n      ]\n    },\n    \"requestedOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the build was started, expressed in Unix time format.\"\n        }\n      ]\n    },\n    \"buildStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusType\"\n        },\n        {\n          \"description\"\
  : \"<p>The status of the build group.</p> <dl> <dt>FAILED</dt> <dd> <p>The build group failed.</p> </dd> <dt>FAULT</dt> <dd> <p>The build group faulted.</p> </dd> <dt>IN_PROGRESS</dt> <dd> <p>The build group is still in progress.</p> </dd> <dt>STOPPED</dt> <dd> <p>The build group stopped.</p> </dd> <dt>SUCCEEDED</dt> <dd> <p>The build group succeeded.</p> </dd> <dt>TIMED_OUT</dt> <dd> <p>The build group timed out.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"primaryArtifact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolvedArtifact\"\n        },\n        {\n          \"description\": \"A <code>ResolvedArtifact</code> object that represents the primary build artifacts for the build group.\"\n        }\n      ]\n    },\n    \"secondaryArtifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolvedSecondaryArtifacts\"\n        },\n        {\n          \"description\": \"An array of <code>ResolvedArtifact</code>\
  \ objects that represents the secondary build artifacts for the build group.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-summary-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildSummary
---
