---
description: Represents the input of an AcknowledgeThirdPartyJob action.
layout: schema
name: AcknowledgeThirdPartyJobInput
properties_list:
- description: ''
  name: jobId
  type: object
- description: ''
  name: nonce
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-acknowledge-third-party-job-input-schema.json
slug: amazon-codepipeline-acknowledge-third-party-job-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-acknowledge-third-party-job-input-schema.json\",\n  \"title\": \"AcknowledgeThirdPartyJobInput\",\n  \"description\": \"Represents the input of an AcknowledgeThirdPartyJob action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ThirdPartyJobId\"\n        },\n        {\n          \"description\": \"The unique system-generated ID of the job.\"\n        }\n      ]\n    },\n    \"nonce\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Nonce\"\n        },\n        {\n          \"description\": \"A system-generated random number that CodePipeline uses to ensure that the job is being worked on by only one job worker. Get this number from the response to a <a>GetThirdPartyJobDetails</a>\
  \ request.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"The clientToken portion of the clientId and clientToken pair used to verify that the calling entity is allowed access to the job and its details.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"nonce\",\n    \"clientToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-acknowledge-third-party-job-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: AcknowledgeThirdPartyJobInput
---
