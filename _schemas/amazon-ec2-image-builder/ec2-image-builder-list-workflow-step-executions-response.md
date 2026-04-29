---
description: ListWorkflowStepExecutionsResponse schema from EC2 Image Builder
layout: schema
name: ListWorkflowStepExecutionsResponse
properties_list:
- description: ''
  name: requestId
  type: object
- description: ''
  name: steps
  type: object
- description: ''
  name: workflowBuildVersionArn
  type: object
- description: ''
  name: workflowExecutionId
  type: object
- description: ''
  name: imageBuildVersionArn
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-list-workflow-step-executions-response-schema.json
slug: ec2-image-builder-list-workflow-step-executions-response
source_filename: ec2-image-builder-list-workflow-step-executions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-workflow-step-executions-response-schema.json\",\n  \"title\": \"ListWorkflowStepExecutionsResponse\",\n  \"description\": \"ListWorkflowStepExecutionsResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"steps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepExecutionsList\"\n        },\n        {\n          \"description\": \"Contains an array of runtime details that represents each step in this runtime instance of the workflow.\"\n       \
  \ }\n      ]\n    },\n    \"workflowBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowBuildVersionArn\"\n        },\n        {\n          \"description\": \"The build version ARN for the Image Builder workflow resource that defines the steps for this runtime instance of the workflow.\"\n        }\n      ]\n    },\n    \"workflowExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionId\"\n        },\n        {\n          \"description\": \"The unique identifier that Image Builder assigned to keep track of runtime details when it ran the workflow.\"\n        }\n      ]\n    },\n    \"imageBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildVersionArn\"\n        },\n        {\n          \"description\": \"The image build version resource ARN that's associated with the specified runtime instance of the workflow.\"\n        }\n   \
  \   ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildMessage\"\n        },\n        {\n          \"description\": \"The output message from the list action, if applicable.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The next token used for paginated responses. When this field isn't empty, there are additional elements that the service has'ot included in this request. Use this token with the next request to retrieve additional objects.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-workflow-step-executions-response-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListWorkflowStepExecutionsResponse
---
