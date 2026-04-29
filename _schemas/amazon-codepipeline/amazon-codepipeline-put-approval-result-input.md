---
description: Represents the input of a <code>PutApprovalResult</code> action.
layout: schema
name: PutApprovalResultInput
properties_list:
- description: ''
  name: pipelineName
  type: object
- description: ''
  name: stageName
  type: object
- description: ''
  name: actionName
  type: object
- description: ''
  name: result
  type: object
- description: ''
  name: token
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-put-approval-result-input-schema.json
slug: amazon-codepipeline-put-approval-result-input
source_filename: amazon-codepipeline-put-approval-result-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-approval-result-input-schema.json\",\n  \"title\": \"PutApprovalResultInput\",\n  \"description\": \"Represents the input of a <code>PutApprovalResult</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline that contains the action. \"\n        }\n      ]\n    },\n    \"stageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageName\"\n        },\n        {\n          \"description\": \"The name of the stage that contains the action.\"\n        }\n      ]\n    },\n    \"actionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionName\"\
  \n        },\n        {\n          \"description\": \"The name of the action for which approval is requested.\"\n        }\n      ]\n    },\n    \"result\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApprovalResult\"\n        },\n        {\n          \"description\": \"Represents information about the result of the approval request.\"\n        }\n      ]\n    },\n    \"token\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApprovalToken\"\n        },\n        {\n          \"description\": \"The system-generated token used to identify a unique approval request. The token for each open approval request can be obtained using the <a>GetPipelineState</a> action. It is used to validate that the approval request corresponding to this token is still valid.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipelineName\",\n    \"stageName\",\n    \"actionName\",\n    \"result\",\n    \"token\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-put-approval-result-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PutApprovalResultInput
---
