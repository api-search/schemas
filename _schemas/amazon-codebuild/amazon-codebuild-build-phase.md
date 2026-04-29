---
description: Information about a stage for a build.
layout: schema
name: BuildPhase
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
schema_file: json-schema/amazon-codebuild-build-phase-schema.json
slug: amazon-codebuild-build-phase
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-phase-schema.json\",\n  \"title\": \"BuildPhase\",\n  \"description\": \"Information about a stage for a build.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"phaseType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildPhaseType\"\n        },\n        {\n          \"description\": \"<p>The name of the build phase. Valid values include:</p> <dl> <dt>BUILD</dt> <dd> <p>Core build activities typically occur in this build phase.</p> </dd> <dt>COMPLETED</dt> <dd> <p>The build has been completed.</p> </dd> <dt>DOWNLOAD_SOURCE</dt> <dd> <p>Source code is being downloaded in this build phase.</p> </dd> <dt>FINALIZING</dt> <dd> <p>The build process is completing in this build phase.</p> </dd> <dt>INSTALL</dt> <dd> <p>Installation activities typically\
  \ occur in this build phase.</p> </dd> <dt>POST_BUILD</dt> <dd> <p>Post-build activities typically occur in this build phase.</p> </dd> <dt>PRE_BUILD</dt> <dd> <p>Pre-build activities typically occur in this build phase.</p> </dd> <dt>PROVISIONING</dt> <dd> <p>The build environment is being set up.</p> </dd> <dt>QUEUED</dt> <dd> <p>The build has been submitted and is queued behind other submitted builds.</p> </dd> <dt>SUBMITTED</dt> <dd> <p>The build has been submitted.</p> </dd> <dt>UPLOAD_ARTIFACTS</dt> <dd> <p>Build output artifacts are being uploaded to the output location.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"phaseStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusType\"\n        },\n        {\n          \"description\": \"<p>The current status of the build phase. Valid values include:</p> <dl> <dt>FAILED</dt> <dd> <p>The build phase failed.</p> </dd> <dt>FAULT</dt> <dd> <p>The build phase faulted.</p> </dd> <dt>IN_PROGRESS</dt>\
  \ <dd> <p>The build phase is still in progress.</p> </dd> <dt>STOPPED</dt> <dd> <p>The build phase stopped.</p> </dd> <dt>SUCCEEDED</dt> <dd> <p>The build phase succeeded.</p> </dd> <dt>TIMED_OUT</dt> <dd> <p>The build phase timed out.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the build phase started, expressed in Unix time format.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"When the build phase ended, expressed in Unix time format.\"\n        }\n      ]\n    },\n    \"durationInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperLong\"\n        },\n        {\n          \"description\": \"How long, in seconds, between the starting and\
  \ ending times of the build's phase.\"\n        }\n      ]\n    },\n    \"contexts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PhaseContexts\"\n        },\n        {\n          \"description\": \"Additional information about a build phase, especially to help troubleshoot a failed build.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-build-phase-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: BuildPhase
---
