---
description: An object that represents an Batch job dependency.
layout: schema
name: BatchJobDependency
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-batch-job-dependency-schema.json
slug: amazon-eventbridge-pipes-batch-job-dependency
source_filename: amazon-eventbridge-pipes-batch-job-dependency-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-job-dependency-schema.json\",\n  \"title\": \"BatchJobDependency\",\n  \"description\": \"An object that represents an Batch job dependency.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The job ID of the Batch job that's associated with this dependency.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchJobDependencyType\"\n        },\n        {\n          \"description\": \"The type of the job dependency.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-job-dependency-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: BatchJobDependency
---
