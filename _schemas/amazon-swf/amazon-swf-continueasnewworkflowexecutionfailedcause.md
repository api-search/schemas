---
description: ''
layout: schema
name: ContinueAsNewWorkflowExecutionFailedCause
properties_list: []
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-continueasnewworkflowexecutionfailedcause-schema.json
slug: amazon-swf-continueasnewworkflowexecutionfailedcause
source_filename: amazon-swf-continueasnewworkflowexecutionfailedcause-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"enum\": [\n    \"UNHANDLED_DECISION\",\n    \"WORKFLOW_TYPE_DEPRECATED\",\n    \"WORKFLOW_TYPE_DOES_NOT_EXIST\",\n    \"DEFAULT_EXECUTION_START_TO_CLOSE_TIMEOUT_UNDEFINED\",\n    \"DEFAULT_TASK_START_TO_CLOSE_TIMEOUT_UNDEFINED\",\n    \"DEFAULT_TASK_LIST_UNDEFINED\",\n    \"DEFAULT_CHILD_POLICY_UNDEFINED\",\n    \"CONTINUE_AS_NEW_WORKFLOW_EXECUTION_RATE_EXCEEDED\",\n    \"OPERATION_NOT_PERMITTED\"\n  ],\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ContinueAsNewWorkflowExecutionFailedCause\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-continueasnewworkflowexecutionfailedcause-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: ContinueAsNewWorkflowExecutionFailedCause
---
