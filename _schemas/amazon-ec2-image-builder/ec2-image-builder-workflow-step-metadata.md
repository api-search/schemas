---
description: Runtime details and status for the workflow step.
layout: schema
name: WorkflowStepMetadata
properties_list:
- description: ''
  name: stepExecutionId
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
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-workflow-step-metadata-schema.json
slug: ec2-image-builder-workflow-step-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-workflow-step-metadata-schema.json\",\n  \"title\": \"WorkflowStepMetadata\",\n  \"description\": \"Runtime details and status for the workflow step.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stepExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepExecutionId\"\n        },\n        {\n          \"description\": \"A unique identifier for the workflow step, assigned at runtime.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepName\"\n        },\n        {\n          \"description\": \"The name of the workflow step.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepDescription\"\
  \n        },\n        {\n          \"description\": \"Description of the workflow step.\"\n        }\n      ]\n    },\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepAction\"\n        },\n        {\n          \"description\": \"The step action name.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepExecutionStatus\"\n        },\n        {\n          \"description\": \"Runtime status for the workflow step.\"\n        }\n      ]\n    },\n    \"rollbackStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepExecutionRollbackStatus\"\n        },\n        {\n          \"description\": \"Reports on the rollback status of the step, if applicable.\"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepMessage\"\n        },\n    \
  \    {\n          \"description\": \"Detailed output message that the workflow step provides at runtime.\"\n        }\n      ]\n    },\n    \"inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepInputs\"\n        },\n        {\n          \"description\": \"Input parameters that Image Builder provides for the workflow step.\"\n        }\n      ]\n    },\n    \"outputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStepOutputs\"\n        },\n        {\n          \"description\": \"The file names that the workflow step created as output for this runtime instance of the workflow.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the workflow step started.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/DateTime\"\n        },\n        {\n          \"description\": \"The timestamp when the workflow step finished.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-workflow-step-metadata-schema.json
tags:
- Amazon Web Services
- Automation
- AWS
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: WorkflowStepMetadata
---
