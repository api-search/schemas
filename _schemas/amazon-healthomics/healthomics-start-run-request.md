---
description: ''
layout: schema
name: StartRunRequest
properties_list:
- description: ''
  name: workflowId
  type: object
- description: ''
  name: workflowType
  type: object
- description: ''
  name: runId
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: runGroupId
  type: object
- description: ''
  name: priority
  type: object
- description: ''
  name: parameters
  type: object
- description: ''
  name: storageCapacity
  type: object
- description: ''
  name: outputUri
  type: object
- description: ''
  name: logLevel
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: requestId
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-start-run-request-schema.json
slug: healthomics-start-run-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-run-request-schema.json\",\n  \"title\": \"StartRunRequest\",\n  \"type\": \"object\",\n  \"required\": [\n    \"roleArn\",\n    \"requestId\"\n  ],\n  \"properties\": {\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\n        },\n        {\n          \"description\": \"The run's workflow ID.\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The run's workflows type.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunId\"\n        },\n        {\n          \"description\": \"The run's ID.\"\n        }\n\
  \      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunRoleArn\"\n        },\n        {\n          \"description\": \"A service role for the run.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunName\"\n        },\n        {\n          \"description\": \"A name for the run.\"\n        }\n      ]\n    },\n    \"runGroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunGroupId\"\n        },\n        {\n          \"description\": \"The run's group ID.\"\n        }\n      ]\n    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartRunRequestPriorityInteger\"\n        },\n        {\n          \"description\": \"A priority for the run.\"\n        }\n      ]\n    },\n    \"parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunParameters\"\
  \n        },\n        {\n          \"description\": \"Parameters for the run.\"\n        }\n      ]\n    },\n    \"storageCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StartRunRequestStorageCapacityInteger\"\n        },\n        {\n          \"description\": \"A storage capacity for the run in gigabytes.\"\n        }\n      ]\n    },\n    \"outputUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunOutputUri\"\n        },\n        {\n          \"description\": \"An output URI for the run.\"\n        }\n      ]\n    },\n    \"logLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunLogLevel\"\n        },\n        {\n          \"description\": \"A log level for the run.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags for the run.\"\n     \
  \   }\n      ]\n    },\n    \"requestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunRequestId\"\n        },\n        {\n          \"description\": \"To ensure that requests don't run multiple times, specify a unique ID for each request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-start-run-request-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: StartRunRequest
---
