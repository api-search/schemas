---
description: ''
layout: schema
name: CountClosedWorkflowExecutionsInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: startTimeFilter
  type: object
- description: ''
  name: closeTimeFilter
  type: object
- description: ''
  name: executionFilter
  type: object
- description: ''
  name: typeFilter
  type: object
- description: ''
  name: tagFilter
  type: object
- description: ''
  name: closeStatusFilter
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-countclosedworkflowexecutionsinput-schema.json
slug: amazon-swf-countclosedworkflowexecutionsinput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\"\n  ],\n  \"title\": \"CountClosedWorkflowExecutionsInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain containing the workflow executions to count.\"\n        }\n      ]\n    },\n    \"startTimeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionTimeFilter\"\n        },\n        {\n          \"description\": \"<p>If specified, only workflow executions that meet the start time criteria of the filter are counted.</p> <note> <p> <code>startTimeFilter</code> and <code>closeTimeFilter</code> are mutually exclusive. You must specify one of these in a request but not both.</p> </note>\"\n        }\n      ]\n    },\n    \"closeTimeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionTimeFilter\"\
  \n        },\n        {\n          \"description\": \"<p>If specified, only workflow executions that meet the close time criteria of the filter are counted.</p> <note> <p> <code>startTimeFilter</code> and <code>closeTimeFilter</code> are mutually exclusive. You must specify one of these in a request but not both.</p> </note>\"\n        }\n      ]\n    },\n    \"executionFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionFilter\"\n        },\n        {\n          \"description\": \"<p>If specified, only workflow executions matching the <code>WorkflowId</code> in the filter are counted.</p> <note> <p> <code>closeStatusFilter</code>, <code>executionFilter</code>, <code>typeFilter</code> and <code>tagFilter</code> are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    },\n    \"typeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowTypeFilter\"\
  \n        },\n        {\n          \"description\": \"<p>If specified, indicates the type of the workflow executions to be counted.</p> <note> <p> <code>closeStatusFilter</code>, <code>executionFilter</code>, <code>typeFilter</code> and <code>tagFilter</code> are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    },\n    \"tagFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagFilter\"\n        },\n        {\n          \"description\": \"<p>If specified, only executions that have a tag that matches the filter are counted.</p> <note> <p> <code>closeStatusFilter</code>, <code>executionFilter</code>, <code>typeFilter</code> and <code>tagFilter</code> are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    },\n    \"closeStatusFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloseStatusFilter\"\n   \
  \     },\n        {\n          \"description\": \"<p>If specified, only workflow executions that match this close status are counted. This filter has an affect only if <code>executionStatus</code> is specified as <code>CLOSED</code>.</p> <note> <p> <code>closeStatusFilter</code>, <code>executionFilter</code>, <code>typeFilter</code> and <code>tagFilter</code> are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-countclosedworkflowexecutionsinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: CountClosedWorkflowExecutionsInput
---
