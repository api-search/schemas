---
description: Represents the output of a <code>PollForThirdPartyJobs</code> action.
layout: schema
name: PollForThirdPartyJobsOutput
properties_list:
- description: ''
  name: jobs
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-poll-for-third-party-jobs-output-schema.json
slug: amazon-codepipeline-poll-for-third-party-jobs-output
source_filename: amazon-codepipeline-poll-for-third-party-jobs-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-poll-for-third-party-jobs-output-schema.json\",\n  \"title\": \"PollForThirdPartyJobsOutput\",\n  \"description\": \"Represents the output of a <code>PollForThirdPartyJobs</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThirdPartyJobList\"\n        },\n        {\n          \"description\": \"Information about the jobs to take action on.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-poll-for-third-party-jobs-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PollForThirdPartyJobsOutput
---
