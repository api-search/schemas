---
description: The details of a job sent in response to a <code>GetThirdPartyJobDetails</code> request.
layout: schema
name: ThirdPartyJobDetails
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
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-third-party-job-details-schema.json
slug: amazon-codepipeline-third-party-job-details
source_filename: amazon-codepipeline-third-party-job-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-third-party-job-details-schema.json\",\n  \"title\": \"ThirdPartyJobDetails\",\n  \"description\": \"The details of a job sent in response to a <code>GetThirdPartyJobDetails</code> request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThirdPartyJobId\"\n        },\n        {\n          \"description\": \"The identifier used to identify the job details in CodePipeline.\"\n        }\n      ]\n    },\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThirdPartyJobData\"\n        },\n        {\n          \"description\": \"The data to be returned by the third party job worker.\"\n        }\n      ]\n    },\n    \"nonce\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/Nonce\"\n        },\n        {\n          \"description\": \"A system-generated random number that CodePipeline uses to ensure that the job is being worked on by only one job worker. Use this number in an <a>AcknowledgeThirdPartyJob</a> request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-third-party-job-details-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ThirdPartyJobDetails
---
