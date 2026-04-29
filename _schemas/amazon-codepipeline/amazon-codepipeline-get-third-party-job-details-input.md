---
description: Represents the input of a <code>GetThirdPartyJobDetails</code> action.
layout: schema
name: GetThirdPartyJobDetailsInput
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-third-party-job-details-input-schema.json
slug: amazon-codepipeline-get-third-party-job-details-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-third-party-job-details-input-schema.json\",\n  \"title\": \"GetThirdPartyJobDetailsInput\",\n  \"description\": \"Represents the input of a <code>GetThirdPartyJobDetails</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThirdPartyJobId\"\n        },\n        {\n          \"description\": \"The unique system-generated ID used for identifying the job.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The clientToken portion of the clientId and clientToken pair used to verify that the calling entity is allowed access to the job\
  \ and its details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-third-party-job-details-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetThirdPartyJobDetailsInput
---
