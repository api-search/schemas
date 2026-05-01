---
description: Represents the input of a <code>GetJobDetails</code> action.
layout: schema
name: GetJobDetailsInput
properties_list:
- description: ''
  name: jobId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-job-details-input-schema.json
slug: amazon-codepipeline-get-job-details-input
source_filename: amazon-codepipeline-get-job-details-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-job-details-input-schema.json\",\n  \"title\": \"GetJobDetailsInput\",\n  \"description\": \"Represents the input of a <code>GetJobDetails</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The unique system-generated ID for the job.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-job-details-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetJobDetailsInput
---
