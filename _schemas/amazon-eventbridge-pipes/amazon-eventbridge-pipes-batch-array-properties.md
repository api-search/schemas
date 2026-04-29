---
description: The array properties for the submitted job, such as the size of the array. The array size can be between 2 and 10,000. If you specify array properties for a job, it becomes an array job. This parameter is used only if the target is an Batch job.
layout: schema
name: BatchArrayProperties
properties_list:
- description: ''
  name: Size
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-batch-array-properties-schema.json
slug: amazon-eventbridge-pipes-batch-array-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-array-properties-schema.json\",\n  \"title\": \"BatchArrayProperties\",\n  \"description\": \"The array properties for the submitted job, such as the size of the array. The array size can be between 2 and 10,000. If you specify array properties for a job, it becomes an array job. This parameter is used only if the target is an Batch job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Size\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchArraySize\"\n        },\n        {\n          \"description\": \"The size of the array, if this is an array batch job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-array-properties-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: BatchArrayProperties
---
