---
description: The details of a target.
layout: schema
name: TargetSummary
properties_list:
- description: ''
  name: Arn
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-target-summary-schema.json
slug: amazon-eventbridge-scheduler-target-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-target-summary-schema.json\",\n  \"title\": \"TargetSummary\",\n  \"description\": \"The details of a target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the target.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-target-summary-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: TargetSummary
---
