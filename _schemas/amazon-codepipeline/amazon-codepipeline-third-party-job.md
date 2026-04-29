---
description: A response to a <code>PollForThirdPartyJobs</code> request returned by CodePipeline when there is a job to be worked on by a partner action.
layout: schema
name: ThirdPartyJob
properties_list:
- description: ''
  name: clientId
  type: object
- description: ''
  name: jobId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-third-party-job-schema.json
slug: amazon-codepipeline-third-party-job
source_filename: amazon-codepipeline-third-party-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-third-party-job-schema.json\",\n  \"title\": \"ThirdPartyJob\",\n  \"description\": \"A response to a <code>PollForThirdPartyJobs</code> request returned by CodePipeline when there is a job to be worked on by a partner action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientId\"\n        },\n        {\n          \"description\": \"The <code>clientToken</code> portion of the <code>clientId</code> and <code>clientToken</code> pair used to verify that the calling entity is allowed access to the job and its details.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"\
  description\": \"The identifier used to identify the job in CodePipeline.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-third-party-job-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ThirdPartyJob
---
