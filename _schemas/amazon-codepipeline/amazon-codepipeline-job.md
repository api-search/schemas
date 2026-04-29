---
description: Represents information about a job.
layout: schema
name: Job
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: data
  type: object
- description: ''
  name: nonce
  type: object
- description: ''
  name: accountId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-job-schema.json
slug: amazon-codepipeline-job
source_filename: amazon-codepipeline-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-job-schema.json\",\n  \"title\": \"Job\",\n  \"description\": \"Represents information about a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The unique system-generated ID of the job.\"\n        }\n      ]\n    },\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobData\"\n        },\n        {\n          \"description\": \"Other data about a job.\"\n        }\n      ]\n    },\n    \"nonce\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Nonce\"\n        },\n        {\n          \"description\": \"A system-generated random number that CodePipeline uses\
  \ to ensure that the job is being worked on by only one job worker. Use this number in an <a>AcknowledgeJob</a> request.\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account to use when performing the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-job-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: Job
---
