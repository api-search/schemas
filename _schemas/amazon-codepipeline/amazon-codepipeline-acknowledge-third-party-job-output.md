---
description: Represents the output of an AcknowledgeThirdPartyJob action.
layout: schema
name: AcknowledgeThirdPartyJobOutput
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-acknowledge-third-party-job-output-schema.json
slug: amazon-codepipeline-acknowledge-third-party-job-output
source_filename: amazon-codepipeline-acknowledge-third-party-job-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-acknowledge-third-party-job-output-schema.json\",\n  \"title\": \"AcknowledgeThirdPartyJobOutput\",\n  \"description\": \"Represents the output of an AcknowledgeThirdPartyJob action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The status information for the third party job, if any.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-acknowledge-third-party-job-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: AcknowledgeThirdPartyJobOutput
---
