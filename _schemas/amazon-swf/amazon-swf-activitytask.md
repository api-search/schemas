---
description: Unit of work sent to an activity worker.
layout: schema
name: ActivityTask
properties_list:
- description: ''
  name: taskToken
  type: object
- description: ''
  name: activityId
  type: object
- description: ''
  name: startedEventId
  type: object
- description: ''
  name: workflowExecution
  type: object
- description: ''
  name: activityType
  type: object
- description: ''
  name: input
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytask-schema.json
slug: amazon-swf-activitytask
source_filename: amazon-swf-activitytask-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"taskToken\",\n    \"activityId\",\n    \"startedEventId\",\n    \"workflowExecution\",\n    \"activityType\"\n  ],\n  \"properties\": {\n    \"taskToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaskToken\"\n        },\n        {\n          \"description\": \"The opaque string used as a handle on the task. This token is used by workers to communicate progress and response information back to the system about the task.\"\n        }\n      ]\n    },\n    \"activityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityId\"\n        },\n        {\n          \"description\": \"The unique ID of the task.\"\n        }\n      ]\n    },\n    \"startedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>ActivityTaskStarted</code> event recorded\
  \ in the history.\"\n        }\n      ]\n    },\n    \"workflowExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"The workflow execution that started this activity task.\"\n        }\n      ]\n    },\n    \"activityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityType\"\n        },\n        {\n          \"description\": \"The type of this activity task.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The inputs provided when the activity task was scheduled. The form of the input is user defined and should be meaningful to the activity implementation.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Unit of work sent to an activity worker.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\
  ,\n  \"title\": \"ActivityTask\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytask-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: ActivityTask
---
