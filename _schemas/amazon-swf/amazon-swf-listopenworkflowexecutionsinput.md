---
description: ''
layout: schema
name: ListOpenWorkflowExecutionsInput
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
  name: nextPageToken
  type: object
- description: ''
  name: maximumPageSize
  type: object
- description: ''
  name: reverseOrder
  type: object
- description: ''
  name: executionFilter
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-listopenworkflowexecutionsinput-schema.json
slug: amazon-swf-listopenworkflowexecutionsinput
source_filename: amazon-swf-listopenworkflowexecutionsinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"startTimeFilter\"\n  ],\n  \"title\": \"ListOpenWorkflowExecutionsInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain that contains the workflow executions to list.\"\n        }\n      ]\n    },\n    \"startTimeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionTimeFilter\"\n        },\n        {\n          \"description\": \"Workflow executions are included in the returned results based on whether their start times are within the range specified by this filter.\"\n        }\n      ]\n    },\n    \"typeFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowTypeFilter\"\n        },\n        {\n          \"description\": \"<p>If specified, only executions of the type\
  \ specified in the filter are returned.</p> <note> <p> <code>executionFilter</code>, <code>typeFilter</code> and <code>tagFilter</code> are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    },\n    \"tagFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagFilter\"\n        },\n        {\n          \"description\": \"<p>If specified, only executions that have the matching tag are listed.</p> <note> <p> <code>executionFilter</code>, <code>typeFilter</code> and <code>tagFilter</code> are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    },\n    \"nextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"<p>If <code>NextPageToken</code> is returned there are more results available. The value of <code>NextPageToken</code> is a unique pagination\
  \ token for each page. Make the call again using the returned token to retrieve the next page. Keep all other arguments unchanged. Each pagination token expires after 24 hours. Using an expired pagination token will return a <code>400</code> error: \\\"<code>Specified token has exceeded its maximum lifetime</code>\\\". </p> <p>The configured <code>maximumPageSize</code> determines how many results can be returned in a single call. </p>\"\n        }\n      ]\n    },\n    \"maximumPageSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of results that are returned per call. Use <code>nextPageToken</code> to obtain further pages of results. \"\n        }\n      ]\n    },\n    \"reverseOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReverseOrder\"\n        },\n        {\n          \"description\": \"When set to <code>true</code>, returns\
  \ the results in reverse order. By default the results are returned in descending order of the start time of the executions.\"\n        }\n      ]\n    },\n    \"executionFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionFilter\"\n        },\n        {\n          \"description\": \"<p>If specified, only workflow executions matching the workflow ID specified in the filter are returned.</p> <note> <p> <code>executionFilter</code>, <code>typeFilter</code> and <code>tagFilter</code> are mutually exclusive. You can specify at most one of these in a request.</p> </note>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-listopenworkflowexecutionsinput-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: ListOpenWorkflowExecutionsInput
---
