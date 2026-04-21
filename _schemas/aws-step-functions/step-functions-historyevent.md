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
tags:
- AWS
- iPaaS
- Orchestration
- Serverless
title: HistoryEvent
---
