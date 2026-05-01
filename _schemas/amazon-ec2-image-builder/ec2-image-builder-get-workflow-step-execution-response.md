---
description: GetWorkflowStepExecutionResponse schema from EC2 Image Builder
layout: schema
name: GetWorkflowStepExecutionResponse
properties_list:
- description: ''
  name: requestId
  type: object
- description: ''
  name: stepExecutionId
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
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: action
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: rollbackStatus
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: inputs
  type: object
- description: ''
  name: outputs
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: onFailure
  type: object
- description: ''
  name: timeoutSeconds
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-get-workflow-step-execution-response-schema.json
slug: ec2-image-builder-get-workflow-step-execution-response
source_filename: ec2-image-builder-get-workflow-step-execution-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-get-workflow-step-execution-response-schema.json\",\n  \"title\": \"GetWorkflowStepExecutionResponse\",\n  \"description\": \"GetWorkflowStepExecutionResponse schema from EC2 Image Builder\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The request ID that uniquely identifies this request.\"\n        }\n      ]\n    },\n    \"stepExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepExecutionId\"\n        },\n        {\n          \"description\": \"The unique identifier for the runtime version of the workflow step that you specified in the request.\"\n        }\n\
  \      ]\n    },\n    \"workflowBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the build version for the Image Builder workflow resource that defines this workflow step.\"\n        }\n      ]\n    },\n    \"workflowExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionId\"\n        },\n        {\n          \"description\": \"The unique identifier that Image Builder assigned to keep track of runtime details when it ran the workflow.\"\n        }\n      ]\n    },\n    \"imageBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the image resource build version that the specified runtime instance of the workflow step creates.\"\
  \n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepName\"\n        },\n        {\n          \"description\": \"The name of the specified runtime instance of the workflow step.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepDescription\"\n        },\n        {\n          \"description\": \"Describes the specified workflow step.\"\n        }\n      ]\n    },\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepAction\"\n        },\n        {\n          \"description\": \"The name of the action that the specified step performs.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepExecutionStatus\"\n        },\n        {\n          \"description\": \"The current status for the specified\
  \ runtime version of the workflow step.\"\n        }\n      ]\n    },\n    \"rollbackStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepExecutionRollbackStatus\"\n        },\n        {\n          \"description\": \"Reports on the rollback status of the specified runtime version of the workflow step, if applicable.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepMessage\"\n        },\n        {\n          \"description\": \"The output message from the specified runtime instance of the workflow step, if applicable.\"\n        }\n      ]\n    },\n    \"inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepInputs\"\n        },\n        {\n          \"description\": \"Input parameters that Image Builder provided for the specified runtime instance of the workflow step.\"\n        }\n      ]\n    },\n    \"outputs\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepOutputs\"\n        },\n        {\n          \"description\": \"The file names that the specified runtime version of the workflow step created as output.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the specified runtime version of the workflow step started.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the specified runtime instance of the workflow step finished.\"\n        }\n      ]\n    },\n    \"onFailure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The action to perform\
  \ if the workflow step fails.\"\n        }\n      ]\n    },\n    \"timeoutSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepTimeoutSecondsInteger\"\n        },\n        {\n          \"description\": \"The maximum duration in seconds for this step to complete its action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-get-workflow-step-execution-response-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: GetWorkflowStepExecutionResponse
---
