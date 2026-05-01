---
description: The retry strategy that's associated with a job. For more information, see <a href="https://docs.aws.amazon.com/batch/latest/userguide/job_retries.html"> Automated job retries</a> in the <i>Batch User Guide</i>.
layout: schema
name: BatchRetryStrategy
properties_list:
- description: ''
  name: Attempts
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-batch-retry-strategy-schema.json
slug: amazon-eventbridge-pipes-batch-retry-strategy
source_filename: amazon-eventbridge-pipes-batch-retry-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-retry-strategy-schema.json\",\n  \"title\": \"BatchRetryStrategy\",\n  \"description\": \"The retry strategy that's associated with a job. For more information, see <a href=\\\"https://docs.aws.amazon.com/batch/latest/userguide/job_retries.html\\\"> Automated job retries</a> in the <i>Batch User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Attempts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchRetryAttempts\"\n        },\n        {\n          \"description\": \"The number of times to move a job to the <code>RUNNABLE</code> status. If the value of <code>attempts</code> is greater than one, the job is retried on failure the same number of attempts as the value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-batch-retry-strategy-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: BatchRetryStrategy
---
