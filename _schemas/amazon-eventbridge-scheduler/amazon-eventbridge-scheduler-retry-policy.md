---
description: A <code>RetryPolicy</code> object that includes information about the retry policy settings, including the maximum age of an event, and the maximum number of times EventBridge Scheduler will try to deliver the event to a target.
layout: schema
name: RetryPolicy
properties_list:
- description: ''
  name: MaximumEventAgeInSeconds
  type: object
- description: ''
  name: MaximumRetryAttempts
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-retry-policy-schema.json
slug: amazon-eventbridge-scheduler-retry-policy
source_filename: amazon-eventbridge-scheduler-retry-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-retry-policy-schema.json\",\n  \"title\": \"RetryPolicy\",\n  \"description\": \"A <code>RetryPolicy</code> object that includes information about the retry policy settings, including the maximum age of an event, and the maximum number of times EventBridge Scheduler will try to deliver the event to a target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaximumEventAgeInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumEventAgeInSeconds\"\n        },\n        {\n          \"description\": \"The maximum amount of time, in seconds, to continue to make retry attempts.\"\n        }\n      ]\n    },\n    \"MaximumRetryAttempts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumRetryAttempts\"\
  \n        },\n        {\n          \"description\": \"The maximum number of retry attempts to make before the request fails. Retry attempts with exponential backoff continue until either the maximum number of attempts is made or until the duration of the <code>MaximumEventAgeInSeconds</code> is reached.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-retry-policy-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: RetryPolicy
---
