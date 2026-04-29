---
description: Represents the input of an AcknowledgeJob action.
layout: schema
name: AcknowledgeJobInput
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: nonce
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-acknowledge-job-input-schema.json
slug: amazon-codepipeline-acknowledge-job-input
source_filename: amazon-codepipeline-acknowledge-job-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-acknowledge-job-input-schema.json\",\n  \"title\": \"AcknowledgeJobInput\",\n  \"description\": \"Represents the input of an AcknowledgeJob action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The unique system-generated ID of the job for which you want to confirm receipt.\"\n        }\n      ]\n    },\n    \"nonce\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Nonce\"\n        },\n        {\n          \"description\": \"A system-generated random number that CodePipeline uses to ensure that the job is being worked on by only one job worker. Get this number from the response of the <a>PollForJobs</a>\
  \ request that returned this job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"nonce\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-acknowledge-job-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: AcknowledgeJobInput
---
