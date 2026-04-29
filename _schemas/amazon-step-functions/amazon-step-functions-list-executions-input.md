---
description: ListExecutionsInput schema from Amazon Step Functions API
layout: schema
name: ListExecutionsInput
properties_list:
- description: ''
  name: stateMachineArn
  type: object
- description: ''
  name: statusFilter
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: mapRunArn
  type: object
provider_name: Amazon Step Functions
provider_slug: amazon-step-functions
schema_file: json-schema/amazon-step-functions-list-executions-input-schema.json
slug: amazon-step-functions-list-executions-input
source_filename: amazon-step-functions-list-executions-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-list-executions-input-schema.json\",\n  \"title\": \"ListExecutionsInput\",\n  \"description\": \"ListExecutionsInput schema from Amazon Step Functions API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stateMachineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the state machine whose executions is listed.</p> <p>You can specify either a <code>mapRunArn</code> or a <code>stateMachineArn</code>, but not both.</p> <p>You can also return a list of executions associated with a specific <a href=\\\"https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-alias.html\\\">alias</a> or <a href=\\\"https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-version.html\\\
  \">version</a>, by specifying an alias ARN or a version ARN in the <code>stateMachineArn</code> parameter.</p>\"\n        }\n      ]\n    },\n    \"statusFilter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionStatus\"\n        },\n        {\n          \"description\": \"If specified, only list the executions whose current execution status matches the given filter.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"<p>The maximum number of results that are returned per call. You can use <code>nextToken</code> to obtain further pages of results. The default is 100 and the maximum allowed page size is 1000. A value of 0 uses the default.</p> <p>This is only an upper limit. The actual number of results returned per call might be fewer than the specified maximum.</p>\"\n        }\n      ]\n    },\n    \"nextToken\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListExecutionsPageToken\"\n        },\n        {\n          \"description\": \"If <code>nextToken</code> is returned, there are more results available. The value of <code>nextToken</code> is a unique pagination token for each page. Make the call again using the returned token to retrieve the next page. Keep all other arguments unchanged. Each pagination token expires after 24 hours. Using an expired pagination token will return an <i>HTTP 400 InvalidToken</i> error.\"\n        }\n      ]\n    },\n    \"mapRunArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the Map Run that started the child workflow executions. If the <code>mapRunArn</code> field is specified, a list of all of the child workflow executions started by a Map Run is returned. For more information, see <a href=\\\
  \"https://docs.aws.amazon.com/step-functions/latest/dg/concepts-examine-map-run.html\\\">Examining Map Run</a> in the <i>Step Functions Developer Guide</i>.</p> <p>You can specify either a <code>mapRunArn</code> or a <code>stateMachineArn</code>, but not both.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-step-functions/refs/heads/main/json-schema/amazon-step-functions-list-executions-input-schema.json
tags:
- AWS
- Orchestration
- Serverless
- State Machine
- Workflow
title: ListExecutionsInput
---
