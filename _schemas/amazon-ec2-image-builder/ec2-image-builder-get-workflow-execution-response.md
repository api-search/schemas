---
description: GetWorkflowExecutionResponse schema from EC2 Image Builder
layout: schema
name: GetWorkflowExecutionResponse
properties_list:
- description: ''
  name: requestId
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
  name: type
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: totalStepCount
  type: object
- description: ''
  name: totalStepsSucceeded
  type: object
- description: ''
  name: totalStepsFailed
  type: object
- description: ''
  name: totalStepsSkipped
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-get-workflow-execution-response-schema.json
slug: ec2-image-builder-get-workflow-execution-response
source_filename: ec2-image-builder-get-workflow-execution-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-get-workflow-execution-response-schema.json\",\n  \"title\": \"GetWorkflowExecutionResponse\",\n  \"description\": \"GetWorkflowExecutionResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"workflowBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the build version for the Image Builder workflow resource that defines the specified runtime\
  \ instance of the workflow.\"\n        }\n      ]\n    },\n    \"workflowExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionId\"\n        },\n        {\n          \"description\": \"The unique identifier that Image Builder assigned to keep track of runtime details when it ran the workflow.\"\n        }\n      ]\n    },\n    \"imageBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image resource build version that the specified runtime instance of the workflow created.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The type of workflow that Image Builder ran for the specified runtime instance of the workflow.\"\n        }\n      ]\n\
  \    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionStatus\"\n        },\n        {\n          \"description\": \"The current runtime status for the specified runtime instance of the workflow.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionMessage\"\n        },\n        {\n          \"description\": \"The output message from the specified runtime instance of the workflow, if applicable.\"\n        }\n      ]\n    },\n    \"totalStepCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepCount\"\n        },\n        {\n          \"description\": \"The total number of steps in the specified runtime instance of the workflow that ran. This number should equal the sum of the step counts for steps that succeeded, were skipped, and failed.\"\n        }\n      ]\n    },\n    \"totalStepsSucceeded\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepCount\"\n        },\n        {\n          \"description\": \"A runtime count for the number of steps that ran successfully in the specified runtime instance of the workflow.\"\n        }\n      ]\n    },\n    \"totalStepsFailed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepCount\"\n        },\n        {\n          \"description\": \"A runtime count for the number of steps that failed in the specified runtime instance of the workflow.\"\n        }\n      ]\n    },\n    \"totalStepsSkipped\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepCount\"\n        },\n        {\n          \"description\": \"A runtime count for the number of steps that were skipped in the specified runtime instance of the workflow.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\
  \n        },\n        {\n          \"description\": \"The timestamp when the specified runtime instance of the workflow started.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the specified runtime instance of the workflow finished.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-get-workflow-execution-response-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: GetWorkflowExecutionResponse
---
