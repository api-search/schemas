---
description: ''
layout: schema
name: CreateWorkflowRequest
properties_list:
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
  name: definitionZip
  type: object
- description: ''
  name: definitionUri
  type: object
- description: ''
  name: main
  type: object
- description: ''
  name: parameterTemplate
  type: object
- description: ''
  name: storageCapacity
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: requestId
  type: object
- description: ''
  name: accelerators
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-create-workflow-request-schema.json
slug: healthomics-create-workflow-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-workflow-request-schema.json\",\n  \"title\": \"CreateWorkflowRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"requestId\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowName\"\n        },\n        {\n          \"description\": \"A name for the workflow.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowDescription\"\n        },\n        {\n          \"description\": \"A description for the workflow.\"\n        }\n      ]\n    },\n    \"engine\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowEngine\"\n        },\n        {\n          \"description\": \"An engine for\
  \ the workflow.\"\n        }\n      ]\n    },\n    \"definitionZip\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Blob\"\n        },\n        {\n          \"description\": \"A ZIP archive for the workflow.\"\n        }\n      ]\n    },\n    \"definitionUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowDefinition\"\n        },\n        {\n          \"description\": \"The URI of a definition for the workflow.\"\n        }\n      ]\n    },\n    \"main\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowMain\"\n        },\n        {\n          \"description\": \"The path of the main definition file for the workflow.\"\n        }\n      ]\n    },\n    \"parameterTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowParameterTemplate\"\n        },\n        {\n          \"description\": \"A parameter template for the workflow.\"\n        }\n\
  \      ]\n    },\n    \"storageCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CreateWorkflowRequestStorageCapacityInteger\"\n        },\n        {\n          \"description\": \"A storage capacity for the workflow in gigabytes.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags for the workflow.\"\n        }\n      ]\n    },\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowRequestId\"\n        },\n        {\n          \"description\": \"To ensure that requests don't run multiple times, specify a unique ID for each request.\"\n        }\n      ]\n    },\n    \"accelerators\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Accelerators\"\n        },\n        {\n          \"description\": \" The computational accelerator specified\
  \ to run the workflow. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-create-workflow-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: CreateWorkflowRequest
---
