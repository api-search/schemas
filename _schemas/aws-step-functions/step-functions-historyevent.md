---
description: Contains details about the events of an execution.
layout: schema
name: HistoryEvent
properties_list:
- description: ''
  name: timestamp
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: previousEventId
  type: object
- description: Contains details about an activity that failed during an execution.
  name: activityFailedEventDetails
  type: object
- description: ''
  name: activityScheduleFailedEventDetails
  type: object
- description: Contains details about an activity scheduled during an execution.
  name: activityScheduledEventDetails
  type: object
- description: Contains details about the start of an activity during an execution.
  name: activityStartedEventDetails
  type: object
- description: Contains details about an activity that successfully terminated during an execution.
  name: activitySucceededEventDetails
  type: object
- description: Contains details about an activity timeout that occurred during an execution.
  name: activityTimedOutEventDetails
  type: object
- description: ''
  name: taskFailedEventDetails
  type: object
- description: ''
  name: taskScheduledEventDetails
  type: object
- description: ''
  name: taskStartFailedEventDetails
  type: object
- description: ''
  name: taskStartedEventDetails
  type: object
- description: ''
  name: taskSubmitFailedEventDetails
  type: object
- description: ''
  name: taskSubmittedEventDetails
  type: object
- description: ''
  name: taskSucceededEventDetails
  type: object
- description: ''
  name: taskTimedOutEventDetails
  type: object
- description: Contains details about an execution failure event.
  name: executionFailedEventDetails
  type: object
- description: Contains details about the start of the execution.
  name: executionStartedEventDetails
  type: object
provider_name: AWS Step Functions
provider_slug: aws-step-functions
schema_file: json-schema/step-functions-historyevent-schema.json
slug: step-functions-historyevent
source_filename: step-functions-historyevent-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HistoryEvent\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {},\n    \"type\": {},\n    \"id\": {},\n    \"previousEventId\": {},\n    \"activityFailedEventDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"error\": {},\n        \"cause\": {}\n      },\n      \"description\": \"Contains details about an activity that failed during an execution.\"\n    },\n    \"activityScheduleFailedEventDetails\": {},\n    \"activityScheduledEventDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"resource\": {},\n        \"input\": {},\n        \"inputDetails\": {},\n        \"timeoutInSeconds\": {},\n        \"heartbeatInSeconds\": {}\n      },\n      \"required\": [\n        \"resource\"\n      ],\n      \"description\": \"Contains details about an activity scheduled during an execution.\"\n    },\n    \"activityStartedEventDetails\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"workerName\": {}\n      },\n      \"description\": \"Contains details about the start of an activity during an execution.\"\n    },\n    \"activitySucceededEventDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"output\": {},\n        \"outputDetails\": {}\n      },\n      \"description\": \"Contains details about an activity that successfully terminated during an execution.\"\n    },\n    \"activityTimedOutEventDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"error\": {},\n        \"cause\": {}\n      },\n      \"description\": \"Contains details about an activity timeout that occurred during an execution.\"\n    },\n    \"taskFailedEventDetails\": {},\n    \"taskScheduledEventDetails\": {},\n    \"taskStartFailedEventDetails\": {},\n    \"taskStartedEventDetails\": {},\n    \"taskSubmitFailedEventDetails\": {},\n    \"taskSubmittedEventDetails\": {},\n    \"taskSucceededEventDetails\"\
  : {},\n    \"taskTimedOutEventDetails\": {},\n    \"executionFailedEventDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"error\": {},\n        \"cause\": {}\n      },\n      \"description\": \"Contains details about an execution failure event.\"\n    },\n    \"executionStartedEventDetails\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"input\": {},\n        \"inputDetails\": {},\n        \"roleArn\": {}\n      },\n      \"description\": \"Contains details about the start of the execution.\"\n    }\n  },\n  \"required\": [\n    \"timestamp\",\n    \"type\",\n    \"id\"\n  ],\n  \"description\": \"Contains details about the events of an execution.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-step-functions/refs/heads/main/json-schema/step-functions-historyevent-schema.json
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: HistoryEvent
---
