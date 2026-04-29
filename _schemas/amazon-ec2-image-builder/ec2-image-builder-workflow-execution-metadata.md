---
description: Metadata that includes details and status from this runtime instance of the workflow.
layout: schema
name: WorkflowExecutionMetadata
properties_list:
- description: ''
  name: workflowBuildVersionArn
  type: object
- description: ''
  name: workflowExecutionId
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
schema_file: json-schema/ec2-image-builder-workflow-execution-metadata-schema.json
slug: ec2-image-builder-workflow-execution-metadata
source_filename: ec2-image-builder-workflow-execution-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-workflow-execution-metadata-schema.json\",\n  \"title\": \"WorkflowExecutionMetadata\",\n  \"description\": \"Metadata that includes details and status from this runtime instance of the workflow.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workflowBuildVersionArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowBuildVersionArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the workflow resource build version that ran.\"\n        }\n      ]\n    },\n    \"workflowExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionId\"\n        },\n        {\n          \"description\": \"Unique identifier that Image Builder assigns to keep track\
  \ of runtime resources each time it runs a workflow.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"Indicates what type of workflow that Image Builder ran for this runtime instance of the workflow.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionStatus\"\n        },\n        {\n          \"description\": \"The current runtime status for this workflow.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowExecutionMessage\"\n        },\n        {\n          \"description\": \"The runtime output message from the workflow, if applicable.\"\n        }\n      ]\n    },\n    \"totalStepCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepCount\"\
  \n        },\n        {\n          \"description\": \"The total number of steps in the workflow. This should equal the sum of the step counts for steps that succeeded, were skipped, and failed.\"\n        }\n      ]\n    },\n    \"totalStepsSucceeded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepCount\"\n        },\n        {\n          \"description\": \"A runtime count for the number of steps in the workflow that ran successfully.\"\n        }\n      ]\n    },\n    \"totalStepsFailed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepCount\"\n        },\n        {\n          \"description\": \"A runtime count for the number of steps in the workflow that failed.\"\n        }\n      ]\n    },\n    \"totalStepsSkipped\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepCount\"\n        },\n        {\n          \"description\": \"A runtime count for the number of\
  \ steps in the workflow that were skipped.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the runtime instance of this workflow started.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The timestamp when this runtime instance of the workflow finished.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-workflow-execution-metadata-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: WorkflowExecutionMetadata
---
