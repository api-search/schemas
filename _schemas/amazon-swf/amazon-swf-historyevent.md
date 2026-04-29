---
description: <p>Event within a workflow execution. A history event can be one of these types:</p> <ul> <li> <p> <code>ActivityTaskCancelRequested</code> – A <code>RequestCancelActivityTask</code> decision was received by the system.</p> </li> <li> <p> <code>ActivityTaskCanceled</code> – The activity task was successfully canceled.</p> </li> <li> <p> <code>ActivityTaskCompleted</code> – An activity worker successfully completed an activity task by calling <a>RespondActivityTaskCompleted</a>.</p> </li> <li> <p> <code>ActivityTaskFailed</code> – An activity worker failed an activity task by calling <a>RespondActivityTaskFailed</a>.</p> </li> <li> <p> <code>ActivityTaskScheduled</code> – An activity task was scheduled for execution.</p> </li> <li> <p> <code>ActivityTaskStarted</code> – The scheduled activity task was dispatched to a worker.</p> </li> <li> <p> <code>ActivityTaskTimedOut</code> – The activity task timed out.</p> </li> <li> <p> <code>CancelTimerFailed</code> – Failed to process
  CancelTimer decision. This happens when the decision isn't configured properly, for example no timer exists with the specified timer Id.</p> </li> <li> <p> <code>CancelWorkflowExecutionFailed</code> – A request to cancel a workflow execution failed.</p> </li> <li> <p> <code>ChildWorkflowExecutionCanceled</code> – A child workflow execution, started by this workflow execution, was canceled and closed.</p> </li> <li> <p> <code>ChildWorkflowExecutionCompleted</code> – A child workflow execution, started by this workflow execution, completed successfully and was closed.</p> </li> <li> <p> <code>ChildWorkflowExecutionFailed</code> – A child workflow execution, started by this workflow execution, failed to complete successfully and was closed.</p> </li> <li> <p> <code>ChildWorkflowExecutionStarted</code> – A child workflow execution was successfully started.</p> </li> <li> <p> <code>ChildWorkflowExecutionTerminated</code> – A child workflow execution, started by this workflow execution, was
  terminated.</p> </li> <li> <p> <code>ChildWorkflowExecutionTimedOut</code> – A child workflow execution, started by this workflow execution, timed out and was closed.</p> </li> <li> <p> <code>CompleteWorkflowExecutionFailed</code> – The workflow execution failed to complete.</p> </li> <li> <p> <code>ContinueAsNewWorkflowExecutionFailed</code> – The workflow execution failed to complete after being continued as a new workflow execution.</p> </li> <li> <p> <code>DecisionTaskCompleted</code> – The decider successfully completed a decision task by calling <a>RespondDecisionTaskCompleted</a>.</p> </li> <li> <p> <code>DecisionTaskScheduled</code> – A decision task was scheduled for the workflow execution.</p> </li> <li> <p> <code>DecisionTaskStarted</code> – The decision task was dispatched to a decider.</p> </li> <li> <p> <code>DecisionTaskTimedOut</code> – The decision task timed out.</p> </li> <li> <p> <code>ExternalWorkflowExecutionCancelRequested</code> – Request to cancel an external workflow
  execution was successfully delivered to the target execution.</p> </li> <li> <p> <code>ExternalWorkflowExecutionSignaled</code> – A signal, requested by this workflow execution, was successfully delivered to the target external workflow execution.</p> </li> <li> <p> <code>FailWorkflowExecutionFailed</code> – A request to mark a workflow execution as failed, itself failed.</p> </li> <li> <p> <code>MarkerRecorded</code> – A marker was recorded in the workflow history as the result of a <code>RecordMarker</code> decision.</p> </li> <li> <p> <code>RecordMarkerFailed</code> – A <code>RecordMarker</code> decision was returned as failed.</p> </li> <li> <p> <code>RequestCancelActivityTaskFailed</code> – Failed to process RequestCancelActivityTask decision. This happens when the decision isn't configured properly.</p> </li> <li> <p> <code>RequestCancelExternalWorkflowExecutionFailed</code> – Request to cancel an external workflow execution failed.</p> </li> <li> <p> <code>RequestCancelExternalWorkflowExecutionInitiated</code>
  – A request was made to request the cancellation of an external workflow execution.</p> </li> <li> <p> <code>ScheduleActivityTaskFailed</code> – Failed to process ScheduleActivityTask decision. This happens when the decision isn't configured properly, for example the activity type specified isn't registered.</p> </li> <li> <p> <code>SignalExternalWorkflowExecutionFailed</code> – The request to signal an external workflow execution failed.</p> </li> <li> <p> <code>SignalExternalWorkflowExecutionInitiated</code> – A request to signal an external workflow was made.</p> </li> <li> <p> <code>StartActivityTaskFailed</code> – A scheduled activity task failed to start.</p> </li> <li> <p> <code>StartChildWorkflowExecutionFailed</code> – Failed to process StartChildWorkflowExecution decision. This happens when the decision isn't configured properly, for example the workflow type specified isn't registered.</p> </li> <li> <p> <code>StartChildWorkflowExecutionInitiated</code> – A request was made
  to start a child workflow execution.</p> </li> <li> <p> <code>StartTimerFailed</code> – Failed to process StartTimer decision. This happens when the decision isn't configured properly, for example a timer already exists with the specified timer Id.</p> </li> <li> <p> <code>TimerCanceled</code> – A timer, previously started for this workflow execution, was successfully canceled.</p> </li> <li> <p> <code>TimerFired</code> – A timer, previously started for this workflow execution, fired.</p> </li> <li> <p> <code>TimerStarted</code> – A timer was started for the workflow execution due to a <code>StartTimer</code> decision.</p> </li> <li> <p> <code>WorkflowExecutionCancelRequested</code> – A request to cancel this workflow execution was made.</p> </li> <li> <p> <code>WorkflowExecutionCanceled</code> – The workflow execution was successfully canceled and closed.</p> </li> <li> <p> <code>WorkflowExecutionCompleted</code> – The workflow execution was closed due to successful completion.</p> </li>
  <li> <p> <code>WorkflowExecutionContinuedAsNew</code> – The workflow execution was closed and a new execution of the same type was created with the same workflowId.</p> </li> <li> <p> <code>WorkflowExecutionFailed</code> – The workflow execution closed due to a failure.</p> </li> <li> <p> <code>WorkflowExecutionSignaled</code> – An external signal was received for the workflow execution.</p> </li> <li> <p> <code>WorkflowExecutionStarted</code> – The workflow execution was started.</p> </li> <li> <p> <code>WorkflowExecutionTerminated</code> – The workflow execution was terminated.</p> </li> <li> <p> <code>WorkflowExecutionTimedOut</code> – The workflow execution was closed because a time out was exceeded.</p> </li> </ul>
layout: schema
name: HistoryEvent
properties_list:
- description: ''
  name: eventTimestamp
  type: object
- description: ''
  name: eventType
  type: object
- description: ''
  name: eventId
  type: object
- description: ''
  name: workflowExecutionStartedEventAttributes
  type: object
- description: ''
  name: workflowExecutionCompletedEventAttributes
  type: object
- description: ''
  name: completeWorkflowExecutionFailedEventAttributes
  type: object
- description: ''
  name: workflowExecutionFailedEventAttributes
  type: object
- description: ''
  name: failWorkflowExecutionFailedEventAttributes
  type: object
- description: ''
  name: workflowExecutionTimedOutEventAttributes
  type: object
- description: ''
  name: workflowExecutionCanceledEventAttributes
  type: object
- description: ''
  name: cancelWorkflowExecutionFailedEventAttributes
  type: object
- description: ''
  name: workflowExecutionContinuedAsNewEventAttributes
  type: object
- description: ''
  name: continueAsNewWorkflowExecutionFailedEventAttributes
  type: object
- description: ''
  name: workflowExecutionTerminatedEventAttributes
  type: object
- description: ''
  name: workflowExecutionCancelRequestedEventAttributes
  type: object
- description: ''
  name: decisionTaskScheduledEventAttributes
  type: object
- description: ''
  name: decisionTaskStartedEventAttributes
  type: object
- description: ''
  name: decisionTaskCompletedEventAttributes
  type: object
- description: ''
  name: decisionTaskTimedOutEventAttributes
  type: object
- description: ''
  name: activityTaskScheduledEventAttributes
  type: object
- description: ''
  name: activityTaskStartedEventAttributes
  type: object
- description: ''
  name: activityTaskCompletedEventAttributes
  type: object
- description: ''
  name: activityTaskFailedEventAttributes
  type: object
- description: ''
  name: activityTaskTimedOutEventAttributes
  type: object
- description: ''
  name: activityTaskCanceledEventAttributes
  type: object
- description: ''
  name: activityTaskCancelRequestedEventAttributes
  type: object
- description: ''
  name: workflowExecutionSignaledEventAttributes
  type: object
- description: ''
  name: markerRecordedEventAttributes
  type: object
- description: ''
  name: recordMarkerFailedEventAttributes
  type: object
- description: ''
  name: timerStartedEventAttributes
  type: object
- description: ''
  name: timerFiredEventAttributes
  type: object
- description: ''
  name: timerCanceledEventAttributes
  type: object
- description: ''
  name: startChildWorkflowExecutionInitiatedEventAttributes
  type: object
- description: ''
  name: childWorkflowExecutionStartedEventAttributes
  type: object
- description: ''
  name: childWorkflowExecutionCompletedEventAttributes
  type: object
- description: ''
  name: childWorkflowExecutionFailedEventAttributes
  type: object
- description: ''
  name: childWorkflowExecutionTimedOutEventAttributes
  type: object
- description: ''
  name: childWorkflowExecutionCanceledEventAttributes
  type: object
- description: ''
  name: childWorkflowExecutionTerminatedEventAttributes
  type: object
- description: ''
  name: signalExternalWorkflowExecutionInitiatedEventAttributes
  type: object
- description: ''
  name: externalWorkflowExecutionSignaledEventAttributes
  type: object
- description: ''
  name: signalExternalWorkflowExecutionFailedEventAttributes
  type: object
- description: ''
  name: externalWorkflowExecutionCancelRequestedEventAttributes
  type: object
- description: ''
  name: requestCancelExternalWorkflowExecutionInitiatedEventAttributes
  type: object
- description: ''
  name: requestCancelExternalWorkflowExecutionFailedEventAttributes
  type: object
- description: ''
  name: scheduleActivityTaskFailedEventAttributes
  type: object
- description: ''
  name: requestCancelActivityTaskFailedEventAttributes
  type: object
- description: ''
  name: startTimerFailedEventAttributes
  type: object
- description: ''
  name: cancelTimerFailedEventAttributes
  type: object
- description: ''
  name: startChildWorkflowExecutionFailedEventAttributes
  type: object
- description: ''
  name: lambdaFunctionScheduledEventAttributes
  type: object
- description: ''
  name: lambdaFunctionStartedEventAttributes
  type: object
- description: ''
  name: lambdaFunctionCompletedEventAttributes
  type: object
- description: ''
  name: lambdaFunctionFailedEventAttributes
  type: object
- description: ''
  name: lambdaFunctionTimedOutEventAttributes
  type: object
- description: ''
  name: scheduleLambdaFunctionFailedEventAttributes
  type: object
- description: ''
  name: startLambdaFunctionFailedEventAttributes
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-historyevent-schema.json
slug: amazon-swf-historyevent
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"eventTimestamp\",\n    \"eventType\",\n    \"eventId\"\n  ],\n  \"properties\": {\n    \"eventTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the event occurred.\"\n        }\n      ]\n    },\n    \"eventType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventType\"\n        },\n        {\n          \"description\": \"The type of the history event.\"\n        }\n      ]\n    },\n    \"eventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The system generated ID of the event. This ID uniquely identifies the event with in the workflow execution history.\"\n        }\n      ]\n    },\n    \"workflowExecutionStartedEventAttributes\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/WorkflowExecutionStartedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>WorkflowExecutionStarted</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"workflowExecutionCompletedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionCompletedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>WorkflowExecutionCompleted</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"completeWorkflowExecutionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CompleteWorkflowExecutionFailedEventAttributes\"\n        },\n        {\n          \"description\"\
  : \"If the event is of type <code>CompleteWorkflowExecutionFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"workflowExecutionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>WorkflowExecutionFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"failWorkflowExecutionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailWorkflowExecutionFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>FailWorkflowExecutionFailed</code> then this member is set and provides detailed information about the event.\
  \ It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"workflowExecutionTimedOutEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionTimedOutEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>WorkflowExecutionTimedOut</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"workflowExecutionCanceledEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionCanceledEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>WorkflowExecutionCanceled</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"cancelWorkflowExecutionFailedEventAttributes\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/CancelWorkflowExecutionFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>CancelWorkflowExecutionFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"workflowExecutionContinuedAsNewEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionContinuedAsNewEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>WorkflowExecutionContinuedAsNew</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"continueAsNewWorkflowExecutionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ContinueAsNewWorkflowExecutionFailedEventAttributes\"\
  \n        },\n        {\n          \"description\": \"If the event is of type <code>ContinueAsNewWorkflowExecutionFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"workflowExecutionTerminatedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionTerminatedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>WorkflowExecutionTerminated</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"workflowExecutionCancelRequestedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionCancelRequestedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>WorkflowExecutionCancelRequested</code>\
  \ then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"decisionTaskScheduledEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DecisionTaskScheduledEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>DecisionTaskScheduled</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"decisionTaskStartedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DecisionTaskStartedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>DecisionTaskStarted</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventAttributes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DecisionTaskCompletedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>DecisionTaskCompleted</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"decisionTaskTimedOutEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DecisionTaskTimedOutEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>DecisionTaskTimedOut</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"activityTaskScheduledEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTaskScheduledEventAttributes\"\n        },\n        {\n          \"description\": \"\
  If the event is of type <code>ActivityTaskScheduled</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"activityTaskStartedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTaskStartedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ActivityTaskStarted</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"activityTaskCompletedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTaskCompletedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ActivityTaskCompleted</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n\
  \        }\n      ]\n    },\n    \"activityTaskFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTaskFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ActivityTaskFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"activityTaskTimedOutEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTaskTimedOutEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ActivityTaskTimedOut</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"activityTaskCanceledEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTaskCanceledEventAttributes\"\
  \n        },\n        {\n          \"description\": \"If the event is of type <code>ActivityTaskCanceled</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"activityTaskCancelRequestedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTaskCancelRequestedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ActivityTaskcancelRequested</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"workflowExecutionSignaledEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionSignaledEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>WorkflowExecutionSignaled</code> then this member is set and\
  \ provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"markerRecordedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MarkerRecordedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>MarkerRecorded</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"recordMarkerFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordMarkerFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>DecisionTaskFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"timerStartedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/TimerStartedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>TimerStarted</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"timerFiredEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimerFiredEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>TimerFired</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"timerCanceledEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimerCanceledEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>TimerCanceled</code> then this member is set and provides detailed information about\
  \ the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"startChildWorkflowExecutionInitiatedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartChildWorkflowExecutionInitiatedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>StartChildWorkflowExecutionInitiated</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"childWorkflowExecutionStartedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildWorkflowExecutionStartedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ChildWorkflowExecutionStarted</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"childWorkflowExecutionCompletedEventAttributes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildWorkflowExecutionCompletedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ChildWorkflowExecutionCompleted</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"childWorkflowExecutionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildWorkflowExecutionFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ChildWorkflowExecutionFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"childWorkflowExecutionTimedOutEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildWorkflowExecutionTimedOutEventAttributes\"\
  \n        },\n        {\n          \"description\": \"If the event is of type <code>ChildWorkflowExecutionTimedOut</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"childWorkflowExecutionCanceledEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildWorkflowExecutionCanceledEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ChildWorkflowExecutionCanceled</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"childWorkflowExecutionTerminatedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChildWorkflowExecutionTerminatedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ChildWorkflowExecutionTerminated</code>\
  \ then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"signalExternalWorkflowExecutionInitiatedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalExternalWorkflowExecutionInitiatedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>SignalExternalWorkflowExecutionInitiated</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"externalWorkflowExecutionSignaledEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalWorkflowExecutionSignaledEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ExternalWorkflowExecutionSignaled</code> then this member is set and provides detailed information about the event.\
  \ It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"signalExternalWorkflowExecutionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalExternalWorkflowExecutionFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>SignalExternalWorkflowExecutionFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"externalWorkflowExecutionCancelRequestedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalWorkflowExecutionCancelRequestedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ExternalWorkflowExecutionCancelRequested</code> then this member is set and provides detailed information about the event. It isn't set for other event types. \"\n        }\n      ]\n\
  \    },\n    \"requestCancelExternalWorkflowExecutionInitiatedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestCancelExternalWorkflowExecutionInitiatedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>RequestCancelExternalWorkflowExecutionInitiated</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"requestCancelExternalWorkflowExecutionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestCancelExternalWorkflowExecutionFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>RequestCancelExternalWorkflowExecutionFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"scheduleActivityTaskFailedEventAttributes\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleActivityTaskFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>ScheduleActivityTaskFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"requestCancelActivityTaskFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestCancelActivityTaskFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>RequestCancelActivityTaskFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"startTimerFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartTimerFailedEventAttributes\"\n        },\n      \
  \  {\n          \"description\": \"If the event is of type <code>StartTimerFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"cancelTimerFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CancelTimerFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>CancelTimerFailed</code> then this member is set and provides detailed information about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"startChildWorkflowExecutionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartChildWorkflowExecutionFailedEventAttributes\"\n        },\n        {\n          \"description\": \"If the event is of type <code>StartChildWorkflowExecutionFailed</code> then this member is set and provides detailed information\
  \ about the event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"lambdaFunctionScheduledEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionScheduledEventAttributes\"\n        },\n        {\n          \"description\": \"Provides the details of the <code>LambdaFunctionScheduled</code> event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"lambdaFunctionStartedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionStartedEventAttributes\"\n        },\n        {\n          \"description\": \"Provides the details of the <code>LambdaFunctionStarted</code> event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"lambdaFunctionCompletedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionCompletedEventAttributes\"\n        },\n        {\n          \"description\"\
  : \"Provides the details of the <code>LambdaFunctionCompleted</code> event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"lambdaFunctionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionFailedEventAttributes\"\n        },\n        {\n          \"description\": \"Provides the details of the <code>LambdaFunctionFailed</code> event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"lambdaFunctionTimedOutEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionTimedOutEventAttributes\"\n        },\n        {\n          \"description\": \"Provides the details of the <code>LambdaFunctionTimedOut</code> event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"scheduleLambdaFunctionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduleLambdaFunctionFailedEventAttributes\"\
  \n        },\n        {\n          \"description\": \"Provides the details of the <code>ScheduleLambdaFunctionFailed</code> event. It isn't set for other event types.\"\n        }\n      ]\n    },\n    \"startLambdaFunctionFailedEventAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartLambdaFunctionFailedEventAttributes\"\n        },\n        {\n          \"description\": \"Provides the details of the <code>StartLambdaFunctionFailed</code> event. It isn't set for other event types.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"<p>Event within a workflow execution. A history event can be one of these types:</p> <ul> <li> <p> <code>ActivityTaskCancelRequested</code> \\u2013 A <code>RequestCancelActivityTask</code> decision was received by the system.</p> </li> <li> <p> <code>ActivityTaskCanceled</code> \\u2013 The activity task was successfully canceled.</p> </li> <li> <p> <code>ActivityTaskCompleted</code> \\u2013 An activity worker\
  \ successfully completed an activity task by calling <a>RespondActivityTaskCompleted</a>.</p> </li> <li> <p> <code>ActivityTaskFailed</code> \\u2013 An activity worker failed an activity task by calling <a>RespondActivityTaskFailed</a>.</p> </li> <li> <p> <code>ActivityTaskScheduled</code> \\u2013 An activity task was scheduled for execution.</p> </li> <li> <p> <code>ActivityTaskStarted</code> \\u2013 The scheduled activity task was dispatched to a worker.</p> </li> <li> <p> <code>ActivityTaskTimedOut</code> \\u2013 The activity task timed out.</p> </li> <li> <p> <code>CancelTimerFailed</code> \\u2013 Failed to process CancelTimer decision. This happens when the decision isn't configured properly, for example no timer exists with the specified timer Id.</p> </li> <li> <p> <code>CancelWorkflowExecutionFailed</code> \\u2013 A request to cancel a workflow execution failed.</p> </li> <li> <p> <code>ChildWorkflowExecutionCanceled</code> \\u2013 A child workflow execution, started by this workflow\
  \ execution, was canceled and closed.</p> </li> <li> <p> <code>ChildWorkflowExecutionCompleted</code> \\u2013 A child workflow execution, started by this workflow execution, completed successfully and was closed.</p> </li> <li> <p> <code>ChildWorkflowExecutionFailed</code> \\u2013 A child workflow execution, started by this workflow execution, failed to complete successfully and was closed.</p> </li> <li> <p> <code>ChildWorkflowExecutionStarted</code> \\u2013 A child workflow execution was successfully started.</p> </li> <li> <p> <code>ChildWorkflowExecutionTerminated</code> \\u2013 A child workflow execution, started by this workflow execution, was terminated.</p> </li> <li> <p> <code>ChildWorkflowExecutionTimedOut</code> \\u2013 A child workflow execution, started by this workflow execution, timed out and was closed.</p> </li> <li> <p> <code>CompleteWorkflowExecutionFailed</code> \\u2013 The workflow execution failed to complete.</p> </li> <li> <p> <code>ContinueAsNewWorkflowExecutionFailed</code>\
  \ \\u2013 The workflow execution failed to complete after being continued as a new workflow execution.</p> </li> <li> <p> <code>DecisionTaskCompleted</code> \\u2013 The decider successfully completed a decision task by calling <a>RespondDecisionTaskCompleted</a>.</p> </li> <li> <p> <code>DecisionTaskScheduled</code> \\u2013 A decision task was scheduled for the workflow execution.</p> </li> <li> <p> <code>DecisionTaskStarted</code> \\u2013 The decision task was dispatched to a decider.</p> </li> <li> <p> <code>DecisionTaskTimedOut</code> \\u2013 The decision task timed out.</p> </li> <li> <p> <code>ExternalWorkflowExecutionCancelRequested</code> \\u2013 Request to cancel an external workflow execution was successfully delivered to the target execution.</p> </li> <li> <p> <code>ExternalWorkflowExecutionSignaled</code> \\u2013 A signal, requested by this workflow execution, was successfully delivered to the target external workflow execution.</p> </li> <li> <p> <code>FailWorkflowExecutionFailed</code>\
  \ \\u2013 A request to mark a workflow execution as failed, itself failed.</p> </li> <li> <p> <code>MarkerRecorded</code> \\u2013 A marker was recorded in the workflow history as the result of a <code>RecordMarker</code> decision.</p> </li> <li> <p> <code>RecordMarkerFailed</code> \\u2013 A <code>RecordMarker</code> decision was returned as failed.</p> </li> <li> <p> <code>RequestCancelActivityTaskFailed</code> \\u2013 Failed to process RequestCancelActivityTask decision. This happens when the decision isn't configured properly.</p> </li> <li> <p> <code>RequestCancelExternalWorkflowExecutionFailed</code> \\u2013 Request to cancel an external workflow execution failed.</p> </li> <li> <p> <code>RequestCancelExternalWorkflowExecutionInitiated</code> \\u2013 A request was made to request the cancellation of an external workflow execution.</p> </li> <li> <p> <code>ScheduleActivityTaskFailed</code> \\u2013 Failed to process ScheduleActivityTask decision. This happens when the decision isn't\
  \ configured properly, for example the activity type specified isn't registered.</p> </li> <li> <p> <code>SignalExternalWorkflowExecutionFailed</code> \\u2013 The request to signal an external workflow execution failed.</p> </li> <li> <p> <code>SignalExternalWorkflowExecutionInitiated</code> \\u2013 A request to signal an external workflow was made.</p> </li> <li> <p> <code>StartActivityTaskFailed</code> \\u2013 A scheduled activity task failed to start.</p> </li> <li> <p> <code>StartChildWorkflowExecutionFailed</code> \\u2013 Failed to process StartChildWorkflowExecution decision. This happens when the decision isn't configured properly, for example the workflow type specified isn't registered.</p> </li> <li> <p> <code>StartChildWorkflowExecutionInitiated</code> \\u2013 A request was made to start a child workflow execution.</p> </li> <li> <p> <code>StartTimerFailed</code> \\u2013 Failed to process StartTimer decision. This happens when the decision isn't configured properly, for example\
  \ a timer already exists with the specified timer Id.</p> </li> <li> <p> <code>TimerCanceled</code> \\u2013 A timer, previously started for this workflow execution, was successfully canceled.</p> </li> <li> <p> <code>TimerFired</code> \\u2013 A timer, previously started for this workflow execution, fired.</p> </li> <li> <p> <code>TimerStarted</code> \\u2013 A timer was started for the workflow execution due to a <code>StartTimer</code> decision.</p> </li> <li> <p> <code>WorkflowExecutionCancelRequested</code> \\u2013 A request to cancel this workflow execution was made.</p> </li> <li> <p> <code>WorkflowExecutionCanceled</code> \\u2013 The workflow execution was successfully canceled and closed.</p> </li> <li> <p> <code>WorkflowExecutionCompleted</code> \\u2013 The workflow execution was closed due to successful completion.</p> </li> <li> <p> <code>WorkflowExecutionContinuedAsNew</code> \\u2013 The workflow execution was closed and a new execution of the same type was created with the same\
  \ workflowId.</p> </li> <li> <p> <code>WorkflowExecutionFailed</code> \\u2013 The workflow execution closed due to a failure.</p> </li> <li> <p> <code>WorkflowExecutionSignaled</code> \\u2013 An external signal was received for the workflow execution.</p> </li> <li> <p> <code>WorkflowExecutionStarted</code> \\u2013 The workflow execution was started.</p> </li> <li> <p> <code>WorkflowExecutionTerminated</code> \\u2013 The workflow execution was terminated.</p> </li> <li> <p> <code>WorkflowExecutionTimedOut</code> \\u2013 The workflow execution was closed because a time out was exceeded.</p> </li> </ul>\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"HistoryEvent\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-historyevent-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: HistoryEvent
---
