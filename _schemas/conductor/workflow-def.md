---
description: A Conductor workflow definition that describes the orchestration of tasks, their sequencing, input/output mappings, failure handling, and timeout policies.
layout: schema
name: WorkflowDef
properties_list:
- description: The name of the workflow definition
  name: name
  type: string
- description: Description of the workflow
  name: description
  type: string
- description: The version of the workflow definition
  name: version
  type: integer
- description: The list of tasks in the workflow
  name: tasks
  type: array
- description: List of input parameter names for the workflow
  name: inputParameters
  type: array
- description: Mapping of output parameters
  name: outputParameters
  type: object
- description: Name of the workflow to execute when this workflow fails
  name: failureWorkflow
  type: string
- description: Schema version (currently 2)
  name: schemaVersion
  type: integer
- description: Whether the workflow is restartable
  name: restartable
  type: boolean
- description: Whether to enable workflow status listener
  name: workflowStatusListenerEnabled
  type: boolean
- description: Email of the workflow definition owner
  name: ownerEmail
  type: string
- description: Timeout policy for the workflow
  name: timeoutPolicy
  type: string
- description: Timeout in seconds for the workflow
  name: timeoutSeconds
  type: integer
- description: Workflow level variables
  name: variables
  type: object
- description: Default input template
  name: inputTemplate
  type: object
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/workflow-def.json
slug: workflow-def
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/workflow-def.json\",\n  \"title\": \"WorkflowDef\",\n  \"description\": \"A Conductor workflow definition that describes the orchestration of tasks, their sequencing, input/output mappings, failure handling, and timeout policies.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"tasks\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workflow definition\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the workflow\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version of the workflow definition\",\n      \"default\": 1\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"description\": \"The list of tasks in the workflow\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/WorkflowTask\"\n      }\n    },\n    \"inputParameters\": {\n      \"type\": \"array\",\n      \"description\": \"List of input parameter names for the workflow\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"outputParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Mapping of output parameters\",\n      \"additionalProperties\": true\n    },\n    \"failureWorkflow\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow to execute when this workflow fails\"\n    },\n    \"schemaVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"Schema version (currently 2)\",\n      \"default\": 2\n    },\n    \"restartable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workflow is restartable\",\n      \"default\": true\n    },\n    \"workflowStatusListenerEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable\
  \ workflow status listener\",\n      \"default\": false\n    },\n    \"ownerEmail\": {\n      \"type\": \"string\",\n      \"description\": \"Email of the workflow definition owner\",\n      \"format\": \"email\"\n    },\n    \"timeoutPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Timeout policy for the workflow\",\n      \"enum\": [\n        \"TIME_OUT_WF\",\n        \"ALERT_ONLY\"\n      ]\n    },\n    \"timeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds for the workflow\",\n      \"default\": 0\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"Workflow level variables\",\n      \"additionalProperties\": true\n    },\n    \"inputTemplate\": {\n      \"type\": \"object\",\n      \"description\": \"Default input template\",\n      \"additionalProperties\": true\n    }\n  },\n  \"$defs\": {\n    \"WorkflowTask\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"name\",\n  \
  \      \"taskReferenceName\",\n        \"type\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the task\"\n        },\n        \"taskReferenceName\": {\n          \"type\": \"string\",\n          \"description\": \"Unique reference name for the task within the workflow\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of task\",\n          \"enum\": [\n            \"SIMPLE\",\n            \"DYNAMIC\",\n            \"FORK_JOIN\",\n            \"FORK_JOIN_DYNAMIC\",\n            \"DECISION\",\n            \"SWITCH\",\n            \"JOIN\",\n            \"DO_WHILE\",\n            \"SUB_WORKFLOW\",\n            \"START_WORKFLOW\",\n            \"EVENT\",\n            \"WAIT\",\n            \"HUMAN\",\n            \"HTTP\",\n            \"INLINE\",\n            \"JSON_JQ_TRANSFORM\",\n            \"LAMBDA\",\n            \"SET_VARIABLE\",\n            \"TERMINATE\"\
  ,\n            \"KAFKA_PUBLISH\"\n          ]\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Task description\"\n        },\n        \"inputParameters\": {\n          \"type\": \"object\",\n          \"description\": \"Input parameter mappings\",\n          \"additionalProperties\": true\n        },\n        \"optional\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this task is optional\",\n          \"default\": false\n        },\n        \"startDelay\": {\n          \"type\": \"integer\",\n          \"description\": \"Delay in seconds before starting the task\",\n          \"default\": 0\n        },\n        \"asyncComplete\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the task is completed asynchronously\",\n          \"default\": false\n        },\n        \"retryCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of retries\"\n        },\n\
  \        \"sink\": {\n          \"type\": \"string\",\n          \"description\": \"Sink for EVENT tasks\"\n        },\n        \"subWorkflowParam\": {\n          \"type\": \"object\",\n          \"description\": \"Sub workflow parameters\",\n          \"properties\": {\n            \"name\": {\n              \"type\": \"string\"\n            },\n            \"version\": {\n              \"type\": \"integer\"\n            }\n          }\n        },\n        \"joinOn\": {\n          \"type\": \"array\",\n          \"description\": \"List of task reference names to join on\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"forkTasks\": {\n          \"type\": \"array\",\n          \"description\": \"List of forked task lists\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/$defs/WorkflowTask\"\n            }\n          }\n        },\n        \"decisionCases\": {\n          \"type\"\
  : \"object\",\n          \"description\": \"Decision cases for SWITCH/DECISION tasks\",\n          \"additionalProperties\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/$defs/WorkflowTask\"\n            }\n          }\n        },\n        \"defaultCase\": {\n          \"type\": \"array\",\n          \"description\": \"Default case tasks for SWITCH/DECISION\",\n          \"items\": {\n            \"$ref\": \"#/$defs/WorkflowTask\"\n          }\n        },\n        \"loopCondition\": {\n          \"type\": \"string\",\n          \"description\": \"Loop condition for DO_WHILE tasks\"\n        },\n        \"loopOver\": {\n          \"type\": \"array\",\n          \"description\": \"Tasks to loop over in DO_WHILE\",\n          \"items\": {\n            \"$ref\": \"#/$defs/WorkflowTask\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/workflow-def.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: WorkflowDef
---
