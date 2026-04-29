---
description: ''
layout: schema
name: GetWorkflowExecutionHistoryInput
properties_list:
- description: ''
  name: domain
  type: object
- description: ''
  name: execution
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
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-getworkflowexecutionhistoryinput-schema.json
slug: amazon-swf-getworkflowexecutionhistoryinput
source_filename: amazon-swf-getworkflowexecutionhistoryinput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domain\",\n    \"execution\"\n  ],\n  \"title\": \"GetWorkflowExecutionHistoryInput\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain containing the workflow execution.\"\n        }\n      ]\n    },\n    \"execution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecution\"\n        },\n        {\n          \"description\": \"Specifies the workflow execution for which to return the history.\"\n        }\n      ]\n    },\n    \"nextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"<p>If <code>NextPageToken</code> is returned there are more results available. The value of <code>NextPageToken</code> is a unique pagination token\
  \ for each page. Make the call again using the returned token to retrieve the next page. Keep all other arguments unchanged. Each pagination token expires after 24 hours. Using an expired pagination token will return a <code>400</code> error: \\\"<code>Specified token has exceeded its maximum lifetime</code>\\\". </p> <p>The configured <code>maximumPageSize</code> determines how many results can be returned in a single call. </p>\"\n        }\n      ]\n    },\n    \"maximumPageSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of results that are returned per call. Use <code>nextPageToken</code> to obtain further pages of results. \"\n        }\n      ]\n    },\n    \"reverseOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReverseOrder\"\n        },\n        {\n          \"description\": \"When set to <code>true</code>, returns the events\
  \ in reverse order. By default the results are returned in ascending order of the <code>eventTimeStamp</code> of the events.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-getworkflowexecutionhistoryinput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: GetWorkflowExecutionHistoryInput
---
