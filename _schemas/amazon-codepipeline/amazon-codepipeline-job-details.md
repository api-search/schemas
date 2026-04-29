---
description: Represents information about the details of a job.
layout: schema
name: JobDetails
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: data
  type: object
- description: ''
  name: accountId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-job-details-schema.json
slug: amazon-codepipeline-job-details
source_filename: amazon-codepipeline-job-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-job-details-schema.json\",\n  \"title\": \"JobDetails\",\n  \"description\": \"Represents information about the details of a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The unique system-generated ID of the job.\"\n        }\n      ]\n    },\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobData\"\n        },\n        {\n          \"description\": \"Represents other information about a job required for a job worker to complete the job. \"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n \
  \       },\n        {\n          \"description\": \"The Amazon Web Services account ID associated with the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-job-details-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: JobDetails
---
