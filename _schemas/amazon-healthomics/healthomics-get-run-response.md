---
description: ''
layout: schema
name: GetRunResponse
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
  name: definition
  type: object
- description: ''
  name: digest
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
  name: resourceDigests
  type: object
- description: ''
  name: startedBy
  type: object
- description: ''
  name: creationTime
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: stopTime
  type: object
- description: ''
  name: statusMessage
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: accelerators
  type: object
provider_name: Amazon HealthOmics
provider_slug: amazon-healthomics
schema_file: json-schema/healthomics-get-run-response-schema.json
slug: healthomics-get-run-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-run-response-schema.json\",\n  \"title\": \"GetRunResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunArn\"\n        },\n        {\n          \"description\": \"The run's ARN.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunId\"\n        },\n        {\n          \"description\": \"The run's ID.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunStatus\"\n        },\n        {\n          \"description\": \"The run's status.\"\n        }\n      ]\n    },\n    \"workflowId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowId\"\
  \n        },\n        {\n          \"description\": \"The run's workflow ID.\"\n        }\n      ]\n    },\n    \"workflowType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowType\"\n        },\n        {\n          \"description\": \"The run's workflow type.\"\n        }\n      ]\n    },\n    \"runId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunId\"\n        },\n        {\n          \"description\": \"The run's ID.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunRoleArn\"\n        },\n        {\n          \"description\": \"The run's service role ARN.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunName\"\n        },\n        {\n          \"description\": \"The run's name.\"\n        }\n      ]\n    },\n    \"runGroupId\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/RunGroupId\"\n        },\n        {\n          \"description\": \"The run's group ID.\"\n        }\n      ]\n    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRunResponsePriorityInteger\"\n        },\n        {\n          \"description\": \"The run's priority.\"\n        }\n      ]\n    },\n    \"definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowDefinition\"\n        },\n        {\n          \"description\": \"The run's definition.\"\n        }\n      ]\n    },\n    \"digest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkflowDigest\"\n        },\n        {\n          \"description\": \"The run's digest.\"\n        }\n      ]\n    },\n    \"parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunParameters\"\n        },\n        {\n          \"description\": \"The\
  \ run's parameters.\"\n        }\n      ]\n    },\n    \"storageCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GetRunResponseStorageCapacityInteger\"\n        },\n        {\n          \"description\": \"The run's storage capacity in gigabytes.\"\n        }\n      ]\n    },\n    \"outputUri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunOutputUri\"\n        },\n        {\n          \"description\": \"The run's output URI.\"\n        }\n      ]\n    },\n    \"logLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunLogLevel\"\n        },\n        {\n          \"description\": \"The run's log level.\"\n        }\n      ]\n    },\n    \"resourceDigests\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunResourceDigests\"\n        },\n        {\n          \"description\": \"The run's resource digests.\"\n        }\n      ]\n    },\n    \"startedBy\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunStartedBy\"\n        },\n        {\n          \"description\": \"Who started the run.\"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunTimestamp\"\n        },\n        {\n          \"description\": \"When the run was created.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunTimestamp\"\n        },\n        {\n          \"description\": \"When the run started.\"\n        }\n      ]\n    },\n    \"stopTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunTimestamp\"\n        },\n        {\n          \"description\": \"The run's stop time.\"\n        }\n      ]\n    },\n    \"statusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunStatusMessage\"\n        },\n        {\n \
  \         \"description\": \"The run's status message.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The run's tags.\"\n        }\n      ]\n    },\n    \"accelerators\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Accelerators\"\n        },\n        {\n          \"description\": \" The computational accelerator used to run the workflow. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthomics/refs/heads/main/json-schema/healthomics-get-run-response-schema.json
tags:
- AWS
- Bioinformatics
- Genomics
- Healthcare
- Life Sciences
- Cloud Computing
title: GetRunResponse
---
