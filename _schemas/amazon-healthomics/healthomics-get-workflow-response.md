---
description: ''
layout: schema
name: GetWorkflowResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: engine
  type: object
- description: ''
  name: definition
  type: object
- description: ''
  name: main
  type: object
- description: ''
  name: digest
  type: object
- description: ''
  name: parameterTemplate
  type: object
- description: ''
  name: storageCapacity
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: statusMessage
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: metadata
  type: object
- description: ''
  name: accelerators
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-get-workflow-response-schema.json
slug: healthomics-get-workflow-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-workflow-response-schema.json\",\n  \"title\": \"GetWorkflowResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowArn\"\n        },\n        {\n          \"description\": \"The workflow's ARN.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The workflow's ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStatus\"\n        },\n        {\n          \"description\": \"The workflow's status.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The workflow's type.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowName\"\n        },\n        {\n          \"description\": \"The workflow's name.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowDescription\"\n        },\n        {\n          \"description\": \"The workflow's description.\"\n        }\n      ]\n    },\n    \"engine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowEngine\"\n        },\n        {\n          \"description\": \"The workflow's engine.\"\n        }\n      ]\n    },\n    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowDefinition\"\n        },\n        {\n          \"description\": \"\
  The workflow's definition.\"\n        }\n      ]\n    },\n    \"main\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowMain\"\n        },\n        {\n          \"description\": \"The path of the main definition file for the workflow.\"\n        }\n      ]\n    },\n    \"digest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowDigest\"\n        },\n        {\n          \"description\": \"The workflow's digest.\"\n        }\n      ]\n    },\n    \"parameterTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowParameterTemplate\"\n        },\n        {\n          \"description\": \"The workflow's parameter template.\"\n        }\n      ]\n    },\n    \"storageCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetWorkflowResponseStorageCapacityInteger\"\n        },\n        {\n          \"description\": \"The workflow's storage capacity\
  \ in gigabytes.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowTimestamp\"\n        },\n        {\n          \"description\": \"When the workflow was created.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowStatusMessage\"\n        },\n        {\n          \"description\": \"The workflow's status message.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The workflow's tags.\"\n        }\n      ]\n    },\n    \"metadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowMetadata\"\n        },\n        {\n          \"description\": \" Gets metadata for workflow. \"\n        }\n      ]\n    },\n    \"accelerators\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/Accelerators\"\n        },\n        {\n          \"description\": \" The computational accelerator specified to run the workflow. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-workflow-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: GetWorkflowResponse
---
