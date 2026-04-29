---
description: Represents the input of a <code>PollForJobs</code> action.
layout: schema
name: PollForJobsInput
properties_list:
- description: ''
  name: actionTypeId
  type: object
- description: ''
  name: maxBatchSize
  type: object
- description: ''
  name: queryParam
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-poll-for-jobs-input-schema.json
slug: amazon-codepipeline-poll-for-jobs-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-poll-for-jobs-input-schema.json\",\n  \"title\": \"PollForJobsInput\",\n  \"description\": \"Represents the input of a <code>PollForJobs</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionTypeId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeId\"\n        },\n        {\n          \"description\": \"Represents information about an action type.\"\n        }\n      ]\n    },\n    \"maxBatchSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxBatchSize\"\n        },\n        {\n          \"description\": \"The maximum number of jobs to return in a poll for jobs call.\"\n        }\n      ]\n    },\n    \"queryParam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/QueryParamMap\"\
  \n        },\n        {\n          \"description\": \"A map of property names and values. For an action type with no queryable properties, this value must be null or an empty map. For an action type with a queryable property, you must supply that property as a key in the map. Only jobs whose action configuration matches the mapped value are returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"actionTypeId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-poll-for-jobs-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PollForJobsInput
---
