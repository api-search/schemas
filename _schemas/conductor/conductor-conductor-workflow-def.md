---
description: ''
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
schema_file: json-schema/conductor-conductor-workflow-def-schema.json
slug: conductor-conductor-workflow-def
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkflowDef\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workflow definition\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the workflow\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The version of the workflow definition\"\n    },\n    \"tasks\": {\n      \"type\": \"array\",\n      \"description\": \"The list of tasks in the workflow\"\n    },\n    \"inputParameters\": {\n      \"type\": \"array\",\n      \"description\": \"List of input parameter names for the workflow\"\n    },\n    \"outputParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Mapping of output parameters\"\n    },\n    \"failureWorkflow\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the workflow to\
  \ execute when this workflow fails\"\n    },\n    \"schemaVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"Schema version (currently 2)\"\n    },\n    \"restartable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workflow is restartable\"\n    },\n    \"workflowStatusListenerEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable workflow status listener\"\n    },\n    \"ownerEmail\": {\n      \"type\": \"string\",\n      \"description\": \"Email of the workflow definition owner\"\n    },\n    \"timeoutPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Timeout policy for the workflow\"\n    },\n    \"timeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in seconds for the workflow\"\n    },\n    \"variables\": {\n      \"type\": \"object\",\n      \"description\": \"Workflow level variables\"\n    },\n    \"inputTemplate\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Default input template\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/conductor/refs/heads/main/json-schema/conductor-conductor-workflow-def-schema.json
tags:
- Automation
- Orchestration
- State
- Tasks
- Workflows
title: WorkflowDef
---
