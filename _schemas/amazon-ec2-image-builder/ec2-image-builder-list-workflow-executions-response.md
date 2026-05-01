---
description: ListWorkflowExecutionsResponse schema from EC2 Image Builder
layout: schema
name: ListWorkflowExecutionsResponse
properties_list:
- description: ''
  name: requestId
  type: object
- description: ''
  name: workflowExecutions
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
schema_file: json-schema/ec2-image-builder-list-workflow-executions-response-schema.json
slug: ec2-image-builder-list-workflow-executions-response
source_filename: ec2-image-builder-list-workflow-executions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-workflow-executions-response-schema.json\",\n  \"title\": \"ListWorkflowExecutionsResponse\",\n  \"description\": \"ListWorkflowExecutionsResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"workflowExecutions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionsList\"\n        },\n        {\n          \"description\": \"Contains an array of runtime details that represents each time a workflow ran for the requested image build version.\"\n\
  \        }\n      ]\n    },\n    \"imageBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildVersionArn\"\n        },\n        {\n          \"description\": \"The resource ARN of the image build version for which you requested a list of workflow runtime details.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildMessage\"\n        },\n        {\n          \"description\": \"The output message from the list action, if applicable.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"The next token used for paginated responses. When this field isn't empty, there are additional elements that the service has'ot included in this request. Use this token with the next request to retrieve additional objects.\"\n     \
  \   }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-list-workflow-executions-response-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: ListWorkflowExecutionsResponse
---
