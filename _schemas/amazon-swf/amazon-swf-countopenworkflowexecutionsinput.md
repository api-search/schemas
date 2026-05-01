---
description: ''
layout: schema
name: CountOpenWorkflowExecutionsInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: startTimeFilter
  type: object
- description: ''
  name: typeFilter
  type: object
- description: ''
  name: tagFilter
  type: object
- description: ''
  name: executionFilter
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-countopenworkflowexecutionsinput-schema.json
slug: amazon-swf-countopenworkflowexecutionsinput
source_filename: amazon-swf-countopenworkflowexecutionsinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"startTimeFilter\"\n  ],\n  \"title\": \"CountOpenWorkflowExecutionsInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain containing the workflow executions to count.\"\n        }\n      ]\n    },\n    \"startTimeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionTimeFilter\"\n        },\n        {\n          \"description\": \"Specifies the start time criteria that workflow executions must meet in order to be counted.\"\n        }\n      ]\n    },\n    \"typeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowTypeFilter\"\n        },\n        {\n          \"description\": \"<p>Specifies the type of the workflow executions to be counted.</p> <note> <p> <code>executionFilter</code>,\
  \ <code>typeFilter</code> and <code>tagFilter</code> are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    },\n    \"tagFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagFilter\"\n        },\n        {\n          \"description\": \"<p>If specified, only executions that have a tag that matches the filter are counted.</p> <note> <p> <code>executionFilter</code>, <code>typeFilter</code> and <code>tagFilter</code> are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    },\n    \"executionFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionFilter\"\n        },\n        {\n          \"description\": \"<p>If specified, only workflow executions matching the <code>WorkflowId</code> in the filter are counted.</p> <note> <p> <code>executionFilter</code>, <code>typeFilter</code> and <code>tagFilter</code>\
  \ are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-countopenworkflowexecutionsinput-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: CountOpenWorkflowExecutionsInput
---
