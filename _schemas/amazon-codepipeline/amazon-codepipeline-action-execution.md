---
description: Represents information about the run of an action.
layout: schema
name: ActionExecution
properties_list:
- description: ''
  name: actionExecutionId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: summary
  type: object
- description: ''
  name: lastStatusChange
  type: object
- description: ''
  name: token
  type: object
- description: ''
  name: lastUpdatedBy
  type: object
- description: ''
  name: externalExecutionId
  type: object
- description: ''
  name: externalExecutionUrl
  type: object
- description: ''
  name: percentComplete
  type: object
- description: ''
  name: errorDetails
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-execution-schema.json
slug: amazon-codepipeline-action-execution
source_filename: amazon-codepipeline-action-execution-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-schema.json\",\n  \"title\": \"ActionExecution\",\n  \"description\": \"Represents information about the run of an action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionId\"\n        },\n        {\n          \"description\": \"<p>ID of the workflow action execution in the current stage. Use the <a>GetPipelineState</a> action to retrieve the current action execution details of the current stage.</p> <note> <p>For older executions, this field might be empty. The action execution ID is available for executions run on or after March 2020.</p> </note>\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/ActionExecutionStatus\"\n        },\n        {\n          \"description\": \"The status of the action, or for a completed action, the last status of the action.\"\n        }\n      ]\n    },\n    \"summary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionSummary\"\n        },\n        {\n          \"description\": \"A summary of the run of the action.\"\n        }\n      ]\n    },\n    \"lastStatusChange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last status change of the action.\"\n        }\n      ]\n    },\n    \"token\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionToken\"\n        },\n        {\n          \"description\": \"The system-generated token used to identify a unique approval request. The token for each open approval request can be obtained using the <code>GetPipelineState</code>\
  \ command. It is used to validate that the approval request corresponding to this token is still valid.\"\n        }\n      ]\n    },\n    \"lastUpdatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedBy\"\n        },\n        {\n          \"description\": \"The ARN of the user who last changed the pipeline.\"\n        }\n      ]\n    },\n    \"externalExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExecutionId\"\n        },\n        {\n          \"description\": \"The external ID of the run of the action.\"\n        }\n      ]\n    },\n    \"externalExecutionUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The URL of a resource external to Amazon Web Services that is used when running the action (for example, an external repository URL).\"\n        }\n      ]\n    },\n    \"percentComplete\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"A percentage of completeness of the action as it runs.\"\n        }\n      ]\n    },\n    \"errorDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorDetails\"\n        },\n        {\n          \"description\": \"The details of an error returned by a URL external to Amazon Web Services.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionExecution
---
