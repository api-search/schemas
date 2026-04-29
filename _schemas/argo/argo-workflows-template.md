---
description: A workflow template definition
layout: schema
name: Template
properties_list:
- description: Name of the template
  name: name
  type: string
- description: ''
  name: inputs
  type: object
- description: ''
  name: outputs
  type: object
- description: Container to run
  name: container
  type: object
- description: Script to run in a container
  name: script
  type: object
- description: Kubernetes resource to create/patch/delete
  name: resource
  type: object
- description: DAG template definition
  name: dag
  type: object
- description: Steps template definition (list of parallel step groups)
  name: steps
  type: array
- description: Suspend template for manual approval
  name: suspend
  type: object
- description: ''
  name: activeDeadlineSeconds
  type: integer
- description: ''
  name: retryStrategy
  type: object
- description: ''
  name: nodeSelector
  type: object
- description: Metadata to set on step pods
  name: metadata
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-template-schema.json
slug: argo-workflows-template
source_filename: argo-workflows-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-template-schema.json\",\n  \"title\": \"Template\",\n  \"description\": \"A workflow template definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the template\"\n    },\n    \"inputs\": {\n      \"$ref\": \"#/components/schemas/Inputs\"\n    },\n    \"outputs\": {\n      \"$ref\": \"#/components/schemas/Outputs\"\n    },\n    \"container\": {\n      \"type\": \"object\",\n      \"description\": \"Container to run\",\n      \"properties\": {\n        \"image\": {\n          \"type\": \"string\"\n        },\n        \"command\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"args\": {\n          \"type\": \"array\",\n          \"items\"\
  : {\n            \"type\": \"string\"\n          }\n        },\n        \"env\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"resources\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"limits\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"type\": \"string\"\n              }\n            },\n            \"requests\": {\n              \"type\": \"object\",\n              \"additionalProperties\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"volumeMounts\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n\
  \          }\n        }\n      }\n    },\n    \"script\": {\n      \"type\": \"object\",\n      \"description\": \"Script to run in a container\",\n      \"properties\": {\n        \"image\": {\n          \"type\": \"string\"\n        },\n        \"command\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"source\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"resource\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes resource to create/patch/delete\",\n      \"properties\": {\n        \"action\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"get\",\n            \"create\",\n            \"apply\",\n            \"delete\",\n            \"replace\",\n            \"patch\"\n          ]\n        },\n        \"manifest\": {\n          \"type\": \"string\"\n        },\n        \"successCondition\": {\n          \"type\": \"string\"\n        },\n\
  \        \"failureCondition\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"dag\": {\n      \"type\": \"object\",\n      \"description\": \"DAG template definition\",\n      \"properties\": {\n        \"tasks\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/DAGTask\"\n          }\n        }\n      }\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Steps template definition (list of parallel step groups)\",\n      \"items\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"$ref\": \"#/components/schemas/WorkflowStep\"\n        }\n      }\n    },\n    \"suspend\": {\n      \"type\": \"object\",\n      \"description\": \"Suspend template for manual approval\",\n      \"properties\": {\n        \"duration\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"activeDeadlineSeconds\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n\
  \    },\n    \"retryStrategy\": {\n      \"$ref\": \"#/components/schemas/RetryStrategy\"\n    },\n    \"nodeSelector\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata to set on step pods\",\n      \"properties\": {\n        \"labels\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-template-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Template
---
