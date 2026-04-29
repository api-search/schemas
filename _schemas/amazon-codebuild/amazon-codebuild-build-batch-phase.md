---
description: Contains information about a stage for a batch build.
layout: schema
name: BuildBatchPhase
properties_list:
- description: ''
  name: phaseType
  type: object
- description: ''
  name: phaseStatus
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: durationInSeconds
  type: object
- description: ''
  name: contexts
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-build-batch-phase-schema.json
slug: amazon-codebuild-build-batch-phase
source_filename: amazon-codebuild-build-batch-phase-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-batch-phase-schema.json\",\n  \"title\": \"BuildBatchPhase\",\n  \"description\": \"Contains information about a stage for a batch build.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phaseType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildBatchPhaseType\"\n        },\n        {\n          \"description\": \"<p>The name of the batch build phase. Valid values include:</p> <dl> <dt>COMBINE_ARTIFACTS</dt> <dd> <p>Build output artifacts are being combined and uploaded to the output location.</p> </dd> <dt>DOWNLOAD_BATCHSPEC</dt> <dd> <p>The batch build specification is being downloaded.</p> </dd> <dt>FAILED</dt> <dd> <p>One or more of the builds failed.</p> </dd> <dt>IN_PROGRESS</dt> <dd> <p>The batch build is in progress.</p> </dd> <dt>STOPPED</dt>\
  \ <dd> <p>The batch build was stopped.</p> </dd> <dt>SUBMITTED</dt> <dd> <p>The btach build has been submitted.</p> </dd> <dt>SUCCEEDED</dt> <dd> <p>The batch build succeeded.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"phaseStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusType\"\n        },\n        {\n          \"description\": \"<p>The current status of the batch build phase. Valid values include:</p> <dl> <dt>FAILED</dt> <dd> <p>The build phase failed.</p> </dd> <dt>FAULT</dt> <dd> <p>The build phase faulted.</p> </dd> <dt>IN_PROGRESS</dt> <dd> <p>The build phase is still in progress.</p> </dd> <dt>STOPPED</dt> <dd> <p>The build phase stopped.</p> </dd> <dt>SUCCEEDED</dt> <dd> <p>The build phase succeeded.</p> </dd> <dt>TIMED_OUT</dt> <dd> <p>The build phase timed out.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n      \
  \  },\n        {\n          \"description\": \"When the batch build phase started, expressed in Unix time format.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the batch build phase ended, expressed in Unix time format.\"\n        }\n      ]\n    },\n    \"durationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperLong\"\n        },\n        {\n          \"description\": \"How long, in seconds, between the starting and ending times of the batch build's phase.\"\n        }\n      ]\n    },\n    \"contexts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PhaseContexts\"\n        },\n        {\n          \"description\": \"Additional information about the batch build phase. Especially to help troubleshoot a failed batch build.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-batch-phase-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildBatchPhase
---
