---
description: Represents the input of a <code>PollForThirdPartyJobs</code> action.
layout: schema
name: PollForThirdPartyJobsInput
properties_list:
- description: ''
  name: actionTypeId
  type: object
- description: ''
  name: maxBatchSize
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-poll-for-third-party-jobs-input-schema.json
slug: amazon-codepipeline-poll-for-third-party-jobs-input
source_filename: amazon-codepipeline-poll-for-third-party-jobs-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-poll-for-third-party-jobs-input-schema.json\",\n  \"title\": \"PollForThirdPartyJobsInput\",\n  \"description\": \"Represents the input of a <code>PollForThirdPartyJobs</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeId\"\n        },\n        {\n          \"description\": \"Represents information about an action type.\"\n        }\n      ]\n    },\n    \"maxBatchSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxBatchSize\"\n        },\n        {\n          \"description\": \"The maximum number of jobs to return in a poll for jobs call.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"actionTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-poll-for-third-party-jobs-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PollForThirdPartyJobsInput
---
