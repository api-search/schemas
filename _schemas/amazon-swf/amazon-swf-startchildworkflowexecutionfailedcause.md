---
description: ''
layout: schema
name: StartChildWorkflowExecutionFailedCause
properties_list: []
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-startchildworkflowexecutionfailedcause-schema.json
slug: amazon-swf-startchildworkflowexecutionfailedcause
source_filename: amazon-swf-startchildworkflowexecutionfailedcause-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"string\",\n  \"enum\": [\n    \"WORKFLOW_TYPE_DOES_NOT_EXIST\",\n    \"WORKFLOW_TYPE_DEPRECATED\",\n    \"OPEN_CHILDREN_LIMIT_EXCEEDED\",\n    \"OPEN_WORKFLOWS_LIMIT_EXCEEDED\",\n    \"CHILD_CREATION_RATE_EXCEEDED\",\n    \"WORKFLOW_ALREADY_RUNNING\",\n    \"DEFAULT_EXECUTION_START_TO_CLOSE_TIMEOUT_UNDEFINED\",\n    \"DEFAULT_TASK_LIST_UNDEFINED\",\n    \"DEFAULT_TASK_START_TO_CLOSE_TIMEOUT_UNDEFINED\",\n    \"DEFAULT_CHILD_POLICY_UNDEFINED\",\n    \"OPERATION_NOT_PERMITTED\"\n  ],\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"StartChildWorkflowExecutionFailedCause\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-startchildworkflowexecutionfailedcause-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: StartChildWorkflowExecutionFailedCause
---
