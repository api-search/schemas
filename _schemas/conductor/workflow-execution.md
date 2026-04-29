---
description: A Conductor workflow execution instance representing a running or completed workflow, including its status, input/output data, task executions, timing information, and failure details.
layout: schema
name: WorkflowExecution
properties_list:
- description: Unique workflow instance ID
  name: workflowId
  type: string
- description: Name of the workflow definition
  name: workflowName
  type: string
- description: Version of the workflow definition
  name: workflowVersion
  type: integer
- description: Correlation ID
  name: correlationId
  type: string
- description: Current status of the workflow
  name: status
  type: string
- description: Start time in epoch milliseconds
  name: startTime
  type: integer
- description: End time in epoch milliseconds
  name: endTime
  type: integer
- description: Last update time in epoch milliseconds
  name: updateTime
  type: integer
- description: Workflow input
  name: input
  type: object
- description: Workflow output
  name: output
  type: object
- description: List of tasks in the workflow execution
  name: tasks
  type: array
- description: Reason for failure or termination
  name: reasonForIncompletion
  type: string
- description: List of failed task reference names
  name: failedReferenceTaskNames
  type: array
- description: The workflow definition used for this execution
  name: workflowDefinition
  type: object
- description: Workflow priority
  name: priority
  type: integer
- description: Workflow variables
  name: variables
  type: object
- description: Last retry timestamp in epoch milliseconds
  name: lastRetriedTime
  type: integer
- description: Owner application
  name: ownerApp
  type: string
- description: Creation timestamp in epoch milliseconds
  name: createTime
  type: integer
- description: Created by
  name: createdBy
  type: string
- description: Parent workflow ID if this is a sub-workflow
  name: parentWorkflowId
  type: string
provider_name: Conductor
provider_slug: conductor
schema_file: json-schema/workflow-execution.json
slug: workflow-execution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/workflow-execution.json\",\n  \"title\": \"WorkflowExecution\",\n  \"description\": \"A Conductor workflow execution instance representing a running or completed workflow, including its status, input/output data, task executions, timing information, and failure details.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workflowId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique workflow instance ID\"\n    },\n    \"workflowName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow definition\"\n    },\n    \"workflowVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"Version of the workflow definition\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation ID\"\n    },\n    \"status\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Current status of the workflow\",\n      \"enum\": [\n        \"RUNNING\",\n        \"COMPLETED\",\n        \"FAILED\",\n        \"TIMED_OUT\",\n        \"TERMINATED\",\n        \"PAUSED\"\n      ]\n    },\n    \"startTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Start time in epoch milliseconds\"\n    },\n    \"endTime\": {\n      \"type\": \"integer\",\n      \"description\": \"End time in epoch milliseconds\"\n    },\n    \"updateTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last update time in epoch milliseconds\"\n    },\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"Workflow input\",\n      \"additionalProperties\": true\n    },\n    \"output\": {\n      \"type\": \"object\",\n      \"description\": \"Workflow output\",\n      \"additionalProperties\": true\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"description\": \"List of tasks in the workflow\
  \ execution\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Task\"\n      }\n    },\n    \"reasonForIncompletion\": {\n      \"type\": \"string\",\n      \"description\": \"Reason for failure or termination\"\n    },\n    \"failedReferenceTaskNames\": {\n      \"type\": \"array\",\n      \"description\": \"List of failed task reference names\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"workflowDefinition\": {\n      \"type\": \"object\",\n      \"description\": \"The workflow definition used for this execution\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"Workflow priority\"\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"Workflow variables\",\n      \"additionalProperties\": true\n    },\n    \"lastRetriedTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Last retry timestamp in epoch milliseconds\"\n    },\n    \"ownerApp\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Owner application\"\n    },\n    \"createTime\": {\n      \"type\": \"integer\",\n      \"description\": \"Creation timestamp in epoch milliseconds\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"Created by\"\n    },\n    \"parentWorkflowId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent workflow ID if this is a sub-workflow\"\n    }\n  },\n  \"$defs\": {\n    \"Task\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"taskId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique task instance ID\"\n        },\n        \"taskType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of the task\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current status of the task\",\n          \"enum\": [\n            \"IN_PROGRESS\",\n            \"CANCELED\",\n            \"FAILED\",\n            \"FAILED_WITH_TERMINAL_ERROR\"\
  ,\n            \"COMPLETED\",\n            \"COMPLETED_WITH_ERRORS\",\n            \"SCHEDULED\",\n            \"TIMED_OUT\",\n            \"SKIPPED\"\n          ]\n        },\n        \"referenceTaskName\": {\n          \"type\": \"string\",\n          \"description\": \"Reference name of the task in the workflow\"\n        },\n        \"workflowInstanceId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the workflow instance this task belongs to\"\n        },\n        \"workflowType\": {\n          \"type\": \"string\",\n          \"description\": \"Type/name of the workflow\"\n        },\n        \"correlationId\": {\n          \"type\": \"string\",\n          \"description\": \"Correlation ID\"\n        },\n        \"scheduledTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Scheduled time in epoch milliseconds\"\n        },\n        \"startTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Start time in epoch\
  \ milliseconds\"\n        },\n        \"endTime\": {\n          \"type\": \"integer\",\n          \"description\": \"End time in epoch milliseconds\"\n        },\n        \"updateTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Last update time in epoch milliseconds\"\n        },\n        \"retryCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Current retry count\"\n        },\n        \"pollCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of times this task was polled\"\n        },\n        \"callbackAfterSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"Callback delay in seconds\"\n        },\n        \"workerId\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the worker that polled this task\"\n        },\n        \"inputData\": {\n          \"type\": \"object\",\n          \"description\": \"Task input data\",\n          \"additionalProperties\": true\n\
  \        },\n        \"outputData\": {\n          \"type\": \"object\",\n          \"description\": \"Task output data\",\n          \"additionalProperties\": true\n        },\n        \"reasonForIncompletion\": {\n          \"type\": \"string\",\n          \"description\": \"Reason for failure\"\n        },\n        \"logs\": {\n          \"type\": \"array\",\n          \"description\": \"Task execution logs\",\n          \"items\": {\n            \"$ref\": \"#/$defs/TaskExecLog\"\n          }\n        },\n        \"domain\": {\n          \"type\": \"string\",\n          \"description\": \"Task domain\"\n        },\n        \"seq\": {\n          \"type\": \"integer\",\n          \"description\": \"Sequence number\"\n        },\n        \"taskDefName\": {\n          \"type\": \"string\",\n          \"description\": \"Task definition name\"\n        },\n        \"responseTimeoutSeconds\": {\n          \"type\": \"integer\",\n          \"description\": \"Response timeout in seconds\"\n \
  \       },\n        \"queueWaitTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Time spent waiting in queue in milliseconds\"\n        }\n      }\n    },\n    \"TaskExecLog\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"log\": {\n          \"type\": \"string\",\n          \"description\": \"Log message\"\n        },\n        \"taskId\": {\n          \"type\": \"string\",\n          \"description\": \"Associated task ID\"\n        },\n        \"createdTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Timestamp of the log entry in epoch milliseconds\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/workflow-execution.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: WorkflowExecution
---
