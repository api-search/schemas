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
- description: ''
  name: activityFailedEventDetails
  type: object
- description: ''
  name: activityScheduleFailedEventDetails
  type: object
- description: ''
  name: activityScheduledEventDetails
  type: object
- description: ''
  name: activityStartedEventDetails
  type: object
- description: ''
  name: activitySucceededEventDetails
  type: object
- description: ''
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
- description: ''
  name: executionFailedEventDetails
  type: object
- description: ''
  name: executionStartedEventDetails
  type: object
- description: ''
  name: executionSucceededEventDetails
  type: object
- description: ''
  name: executionAbortedEventDetails
  type: object
- description: ''
  name: executionTimedOutEventDetails
  type: object
- description: ''
  name: mapStateStartedEventDetails
  type: object
- description: ''
  name: mapIterationStartedEventDetails
  type: object
- description: ''
  name: mapIterationSucceededEventDetails
  type: object
- description: ''
  name: mapIterationFailedEventDetails
  type: object
- description: ''
  name: mapIterationAbortedEventDetails
  type: object
- description: ''
  name: lambdaFunctionFailedEventDetails
  type: object
- description: ''
  name: lambdaFunctionScheduleFailedEventDetails
  type: object
- description: ''
  name: lambdaFunctionScheduledEventDetails
  type: object
- description: ''
  name: lambdaFunctionStartFailedEventDetails
  type: object
- description: ''
  name: lambdaFunctionSucceededEventDetails
  type: object
- description: ''
  name: lambdaFunctionTimedOutEventDetails
  type: object
- description: ''
  name: stateEnteredEventDetails
  type: object
- description: ''
  name: stateExitedEventDetails
  type: object
- description: ''
  name: mapRunStartedEventDetails
  type: object
- description: ''
  name: mapRunFailedEventDetails
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-history-event-schema.json
slug: amazon-step-functions-history-event
source_filename: amazon-step-functions-history-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-history-event-schema.json\",\n  \"title\": \"HistoryEvent\",\n  \"description\": \"Contains details about the events of an execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time the event occurred.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoryEventType\"\n        },\n        {\n          \"description\": \"The type of the event.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The\
  \ id of the event. Events are numbered sequentially, starting at one.\"\n        }\n      ]\n    },\n    \"previousEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The id of the previous event.\"\n        }\n      ]\n    },\n    \"activityFailedEventDetails\": {\n      \"$ref\": \"#/components/schemas/ActivityFailedEventDetails\"\n    },\n    \"activityScheduleFailedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityScheduleFailedEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about an activity schedule event that failed during an execution.\"\n        }\n      ]\n    },\n    \"activityScheduledEventDetails\": {\n      \"$ref\": \"#/components/schemas/ActivityScheduledEventDetails\"\n    },\n    \"activityStartedEventDetails\": {\n      \"$ref\": \"#/components/schemas/ActivityStartedEventDetails\"\n\
  \    },\n    \"activitySucceededEventDetails\": {\n      \"$ref\": \"#/components/schemas/ActivitySucceededEventDetails\"\n    },\n    \"activityTimedOutEventDetails\": {\n      \"$ref\": \"#/components/schemas/ActivityTimedOutEventDetails\"\n    },\n    \"taskFailedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskFailedEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about the failure of a task.\"\n        }\n      ]\n    },\n    \"taskScheduledEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskScheduledEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about a task that was scheduled.\"\n        }\n      ]\n    },\n    \"taskStartFailedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStartFailedEventDetails\"\n        },\n        {\n          \"description\": \"Contains details\
  \ about a task that failed to start.\"\n        }\n      ]\n    },\n    \"taskStartedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskStartedEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about a task that was started.\"\n        }\n      ]\n    },\n    \"taskSubmitFailedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskSubmitFailedEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about a task that where the submit failed.\"\n        }\n      ]\n    },\n    \"taskSubmittedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskSubmittedEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about a submitted task.\"\n        }\n      ]\n    },\n    \"taskSucceededEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskSucceededEventDetails\"\
  \n        },\n        {\n          \"description\": \"Contains details about a task that succeeded.\"\n        }\n      ]\n    },\n    \"taskTimedOutEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskTimedOutEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about a task that timed out.\"\n        }\n      ]\n    },\n    \"executionFailedEventDetails\": {\n      \"$ref\": \"#/components/schemas/ExecutionFailedEventDetails\"\n    },\n    \"executionStartedEventDetails\": {\n      \"$ref\": \"#/components/schemas/ExecutionStartedEventDetails\"\n    },\n    \"executionSucceededEventDetails\": {\n      \"$ref\": \"#/components/schemas/ExecutionSucceededEventDetails\"\n    },\n    \"executionAbortedEventDetails\": {\n      \"$ref\": \"#/components/schemas/ExecutionAbortedEventDetails\"\n    },\n    \"executionTimedOutEventDetails\": {\n      \"$ref\": \"#/components/schemas/ExecutionTimedOutEventDetails\"\n    },\n\
  \    \"mapStateStartedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapStateStartedEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about Map state that was started.\"\n        }\n      ]\n    },\n    \"mapIterationStartedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapIterationEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about an iteration of a Map state that was started.\"\n        }\n      ]\n    },\n    \"mapIterationSucceededEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapIterationEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about an iteration of a Map state that succeeded.\"\n        }\n      ]\n    },\n    \"mapIterationFailedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapIterationEventDetails\"\
  \n        },\n        {\n          \"description\": \"Contains details about an iteration of a Map state that failed.\"\n        }\n      ]\n    },\n    \"mapIterationAbortedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapIterationEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about an iteration of a Map state that was aborted.\"\n        }\n      ]\n    },\n    \"lambdaFunctionFailedEventDetails\": {\n      \"$ref\": \"#/components/schemas/LambdaFunctionFailedEventDetails\"\n    },\n    \"lambdaFunctionScheduleFailedEventDetails\": {\n      \"$ref\": \"#/components/schemas/LambdaFunctionScheduleFailedEventDetails\"\n    },\n    \"lambdaFunctionScheduledEventDetails\": {\n      \"$ref\": \"#/components/schemas/LambdaFunctionScheduledEventDetails\"\n    },\n    \"lambdaFunctionStartFailedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionStartFailedEventDetails\"\
  \n        },\n        {\n          \"description\": \"Contains details about a lambda function that failed to start during an execution.\"\n        }\n      ]\n    },\n    \"lambdaFunctionSucceededEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionSucceededEventDetails\"\n        },\n        {\n          \"description\": \"Contains details about a Lambda function that terminated successfully during an execution.\"\n        }\n      ]\n    },\n    \"lambdaFunctionTimedOutEventDetails\": {\n      \"$ref\": \"#/components/schemas/LambdaFunctionTimedOutEventDetails\"\n    },\n    \"stateEnteredEventDetails\": {\n      \"$ref\": \"#/components/schemas/StateEnteredEventDetails\"\n    },\n    \"stateExitedEventDetails\": {\n      \"$ref\": \"#/components/schemas/StateExitedEventDetails\"\n    },\n    \"mapRunStartedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapRunStartedEventDetails\"\n \
  \       },\n        {\n          \"description\": \"Contains details, such as <code>mapRunArn</code>, and the start date and time of a Map Run. <code>mapRunArn</code> is the Amazon Resource Name (ARN) of the Map Run that was started.\"\n        }\n      ]\n    },\n    \"mapRunFailedEventDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MapRunFailedEventDetails\"\n        },\n        {\n          \"description\": \"Contains error and cause details about a Map Run that failed.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"timestamp\",\n    \"type\",\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-history-event-schema.json
tags:
- Orchestration
- Serverless
- State Machine
- Workflow
title: HistoryEvent
---
