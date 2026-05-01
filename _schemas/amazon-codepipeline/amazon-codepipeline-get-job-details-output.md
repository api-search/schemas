---
description: Represents the output of a <code>GetJobDetails</code> action.
layout: schema
name: GetJobDetailsOutput
properties_list:
- description: ''
  name: jobDetails
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-job-details-output-schema.json
slug: amazon-codepipeline-get-job-details-output
source_filename: amazon-codepipeline-get-job-details-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-job-details-output-schema.json\",\n  \"title\": \"GetJobDetailsOutput\",\n  \"description\": \"Represents the output of a <code>GetJobDetails</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDetails\"\n        },\n        {\n          \"description\": \"<p>The details of the job.</p> <note> <p>If AWSSessionCredentials is used, a long-running job can call <code>GetJobDetails</code> again to obtain new credentials.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-job-details-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetJobDetailsOutput
---
