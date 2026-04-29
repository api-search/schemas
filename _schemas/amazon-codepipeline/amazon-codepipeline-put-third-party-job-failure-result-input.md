---
description: Represents the input of a <code>PutThirdPartyJobFailureResult</code> action.
layout: schema
name: PutThirdPartyJobFailureResultInput
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: clientToken
  type: object
- description: ''
  name: failureDetails
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-put-third-party-job-failure-result-input-schema.json
slug: amazon-codepipeline-put-third-party-job-failure-result-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-third-party-job-failure-result-input-schema.json\",\n  \"title\": \"PutThirdPartyJobFailureResultInput\",\n  \"description\": \"Represents the input of a <code>PutThirdPartyJobFailureResult</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThirdPartyJobId\"\n        },\n        {\n          \"description\": \"The ID of the job that failed. This is the same ID returned from <code>PollForThirdPartyJobs</code>.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The clientToken portion of the clientId and clientToken pair used to verify\
  \ that the calling entity is allowed access to the job and its details.\"\n        }\n      ]\n    },\n    \"failureDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailureDetails\"\n        },\n        {\n          \"description\": \"Represents information about failure details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"clientToken\",\n    \"failureDetails\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-third-party-job-failure-result-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PutThirdPartyJobFailureResultInput
---
