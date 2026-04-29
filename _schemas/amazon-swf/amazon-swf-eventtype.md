---
description: ''
layout: schema
name: EventType
properties_list: []
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-eventtype-schema.json
slug: amazon-swf-eventtype
source_json: "{\n  \"type\": \"string\",\n  \"enum\": [\n    \"WorkflowExecutionStarted\",\n    \"WorkflowExecutionCancelRequested\",\n    \"WorkflowExecutionCompleted\",\n    \"CompleteWorkflowExecutionFailed\",\n    \"WorkflowExecutionFailed\",\n    \"FailWorkflowExecutionFailed\",\n    \"WorkflowExecutionTimedOut\",\n    \"WorkflowExecutionCanceled\",\n    \"CancelWorkflowExecutionFailed\",\n    \"WorkflowExecutionContinuedAsNew\",\n    \"ContinueAsNewWorkflowExecutionFailed\",\n    \"WorkflowExecutionTerminated\",\n    \"DecisionTaskScheduled\",\n    \"DecisionTaskStarted\",\n    \"DecisionTaskCompleted\",\n    \"DecisionTaskTimedOut\",\n    \"ActivityTaskScheduled\",\n    \"ScheduleActivityTaskFailed\",\n    \"ActivityTaskStarted\",\n    \"ActivityTaskCompleted\",\n    \"ActivityTaskFailed\",\n    \"ActivityTaskTimedOut\",\n    \"ActivityTaskCanceled\",\n    \"ActivityTaskCancelRequested\",\n    \"RequestCancelActivityTaskFailed\",\n    \"WorkflowExecutionSignaled\",\n    \"MarkerRecorded\"\
  ,\n    \"RecordMarkerFailed\",\n    \"TimerStarted\",\n    \"StartTimerFailed\",\n    \"TimerFired\",\n    \"TimerCanceled\",\n    \"CancelTimerFailed\",\n    \"StartChildWorkflowExecutionInitiated\",\n    \"StartChildWorkflowExecutionFailed\",\n    \"ChildWorkflowExecutionStarted\",\n    \"ChildWorkflowExecutionCompleted\",\n    \"ChildWorkflowExecutionFailed\",\n    \"ChildWorkflowExecutionTimedOut\",\n    \"ChildWorkflowExecutionCanceled\",\n    \"ChildWorkflowExecutionTerminated\",\n    \"SignalExternalWorkflowExecutionInitiated\",\n    \"SignalExternalWorkflowExecutionFailed\",\n    \"ExternalWorkflowExecutionSignaled\",\n    \"RequestCancelExternalWorkflowExecutionInitiated\",\n    \"RequestCancelExternalWorkflowExecutionFailed\",\n    \"ExternalWorkflowExecutionCancelRequested\",\n    \"LambdaFunctionScheduled\",\n    \"LambdaFunctionStarted\",\n    \"LambdaFunctionCompleted\",\n    \"LambdaFunctionFailed\",\n    \"LambdaFunctionTimedOut\",\n    \"ScheduleLambdaFunctionFailed\"\
  ,\n    \"StartLambdaFunctionFailed\"\n  ],\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"EventType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-eventtype-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: EventType
---
