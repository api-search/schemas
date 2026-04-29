---
description: Contains a paginated list of information about workflow executions.
layout: schema
name: WorkflowExecutionInfos
properties_list:
- description: ''
  name: executionInfos
  type: object
- description: ''
  name: nextPageToken
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-workflowexecutioninfos-schema.json
slug: amazon-swf-workflowexecutioninfos
source_filename: amazon-swf-workflowexecutioninfos-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"executionInfos\"\n  ],\n  \"properties\": {\n    \"executionInfos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionInfoList\"\n        },\n        {\n          \"description\": \"The list of workflow information structures.\"\n        }\n      ]\n    },\n    \"nextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"<p>If a <code>NextPageToken</code> was returned by a previous call, there are more results available. To retrieve the next page of results, make the call again using the returned token in <code>nextPageToken</code>. Keep all other arguments unchanged.</p> <p>The configured <code>maximumPageSize</code> determines how many results can be returned in a single call.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains a paginated list of information\
  \ about workflow executions.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"WorkflowExecutionInfos\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-workflowexecutioninfos-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: WorkflowExecutionInfos
---
