---
description: Represents the output of a <code>GetThirdPartyJobDetails</code> action.
layout: schema
name: GetThirdPartyJobDetailsOutput
properties_list:
- description: ''
  name: jobDetails
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-third-party-job-details-output-schema.json
slug: amazon-codepipeline-get-third-party-job-details-output
source_filename: amazon-codepipeline-get-third-party-job-details-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-third-party-job-details-output-schema.json\",\n  \"title\": \"GetThirdPartyJobDetailsOutput\",\n  \"description\": \"Represents the output of a <code>GetThirdPartyJobDetails</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThirdPartyJobDetails\"\n        },\n        {\n          \"description\": \"The details of the job, including any protected values defined for the job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-third-party-job-details-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetThirdPartyJobDetailsOutput
---
