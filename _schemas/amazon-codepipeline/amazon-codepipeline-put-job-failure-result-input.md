---
description: Represents the input of a <code>PutJobFailureResult</code> action.
layout: schema
name: PutJobFailureResultInput
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: failureDetails
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-put-job-failure-result-input-schema.json
slug: amazon-codepipeline-put-job-failure-result-input
source_filename: amazon-codepipeline-put-job-failure-result-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-job-failure-result-input-schema.json\",\n  \"title\": \"PutJobFailureResultInput\",\n  \"description\": \"Represents the input of a <code>PutJobFailureResult</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The unique system-generated ID of the job that failed. This is the same ID returned from <code>PollForJobs</code>.\"\n        }\n      ]\n    },\n    \"failureDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureDetails\"\n        },\n        {\n          \"description\": \"The details about the failure of a job.\"\n        }\n      ]\n    }\n  },\n  \"required\":\
  \ [\n    \"jobId\",\n    \"failureDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-job-failure-result-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PutJobFailureResultInput
---
