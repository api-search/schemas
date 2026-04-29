---
description: A structure that represents a decision task. Decision tasks are sent to deciders in order for them to make decisions.
layout: schema
name: DecisionTask
properties_list:
- description: ''
  name: taskToken
  type: object
- description: ''
  name: startedEventId
  type: object
- description: ''
  name: workflowExecution
  type: object
- description: ''
  name: workflowType
  type: object
- description: ''
  name: events
  type: object
- description: ''
  name: nextPageToken
  type: object
- description: ''
  name: previousStartedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-decisiontask-schema.json
slug: amazon-swf-decisiontask
source_filename: amazon-swf-decisiontask-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"taskToken\",\n    \"startedEventId\",\n    \"workflowExecution\",\n    \"workflowType\",\n    \"events\"\n  ],\n  \"properties\": {\n    \"taskToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskToken\"\n        },\n        {\n          \"description\": \"The opaque string used as a handle on the task. This token is used by workers to communicate progress and response information back to the system about the task.\"\n        }\n      ]\n    },\n    \"startedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskStarted</code> event recorded in the history.\"\n        }\n      ]\n    },\n    \"workflowExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\":\
  \ \"The workflow execution for which this decision task was created.\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The type of the workflow execution for which this decision task was created.\"\n        }\n      ]\n    },\n    \"events\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoryEventList\"\n        },\n        {\n          \"description\": \"A paginated list of history events of the workflow execution. The decider uses this during the processing of the decision task.\"\n        }\n      ]\n    },\n    \"nextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"<p>If a <code>NextPageToken</code> was returned by a previous call, there are more results available. To retrieve the next page of results,\
  \ make the call again using the returned token in <code>nextPageToken</code>. Keep all other arguments unchanged.</p> <p>The configured <code>maximumPageSize</code> determines how many results can be returned in a single call.</p>\"\n        }\n      ]\n    },\n    \"previousStartedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the DecisionTaskStarted event of the previous decision task of this workflow execution that was processed by the decider. This can be used to determine the events in the history new since the last decision task received by the decider.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"A structure that represents a decision task. Decision tasks are sent to deciders in order for them to make decisions.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DecisionTask\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-decisiontask-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DecisionTask
---
