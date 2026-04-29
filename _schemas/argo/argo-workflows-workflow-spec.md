---
description: Specification of a workflow
layout: schema
name: WorkflowSpec
properties_list:
- description: The name of the entrypoint template
  name: entrypoint
  type: string
- description: ''
  name: arguments
  type: object
- description: List of workflow templates
  name: templates
  type: array
- description: Service account to run workflow pods
  name: serviceAccountName
  type: string
- description: Volumes available to workflow steps
  name: volumes
  type: array
- description: Duration in seconds before workflow times out
  name: activeDeadlineSeconds
  type: integer
- description: ''
  name: nodeSelector
  type: object
- description: ''
  name: tolerations
  type: array
- description: Maximum number of parallel running pods
  name: parallelism
  type: integer
- description: Strategy for cleaning up completed workflows
  name: ttlStrategy
  type: object
- description: Strategy for garbage collecting completed pods
  name: podGC
  type: object
- description: Reference to a WorkflowTemplate
  name: workflowTemplateRef
  type: object
- description: Whether to archive workflow logs
  name: archiveLogs
  type: boolean
- description: Lifecycle hooks for the workflow
  name: hooks
  type: object
- description: Template to execute on workflow exit
  name: onExit
  type: string
- description: ''
  name: retryStrategy
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-workflow-spec-schema.json
slug: argo-workflows-workflow-spec
source_filename: argo-workflows-workflow-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-spec-schema.json\",\n  \"title\": \"WorkflowSpec\",\n  \"description\": \"Specification of a workflow\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"entrypoint\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the entrypoint template\"\n    },\n    \"arguments\": {\n      \"$ref\": \"#/components/schemas/Arguments\"\n    },\n    \"templates\": {\n      \"type\": \"array\",\n      \"description\": \"List of workflow templates\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Template\"\n      }\n    },\n    \"serviceAccountName\": {\n      \"type\": \"string\",\n      \"description\": \"Service account to run workflow pods\"\n    },\n    \"volumes\": {\n      \"type\": \"array\",\n      \"description\": \"Volumes available to workflow steps\",\n\
  \      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"activeDeadlineSeconds\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Duration in seconds before workflow times out\"\n    },\n    \"nodeSelector\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tolerations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"parallelism\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of parallel running pods\"\n    },\n    \"ttlStrategy\": {\n      \"type\": \"object\",\n      \"description\": \"Strategy for cleaning up completed workflows\",\n      \"properties\": {\n        \"secondsAfterCompletion\": {\n          \"type\": \"integer\"\n        },\n        \"secondsAfterSuccess\": {\n          \"type\": \"integer\"\n        },\n        \"secondsAfterFailure\": {\n          \"type\"\
  : \"integer\"\n        }\n      }\n    },\n    \"podGC\": {\n      \"type\": \"object\",\n      \"description\": \"Strategy for garbage collecting completed pods\",\n      \"properties\": {\n        \"strategy\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"OnPodCompletion\",\n            \"OnPodSuccess\",\n            \"OnWorkflowCompletion\",\n            \"OnWorkflowSuccess\"\n          ]\n        }\n      }\n    },\n    \"workflowTemplateRef\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a WorkflowTemplate\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"clusterScope\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"archiveLogs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to archive workflow logs\"\n    },\n    \"hooks\": {\n      \"type\": \"object\",\n      \"description\": \"Lifecycle hooks for the workflow\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"object\"\n      }\n    },\n    \"onExit\": {\n      \"type\": \"string\",\n      \"description\": \"Template to execute on workflow exit\"\n    },\n    \"retryStrategy\": {\n      \"$ref\": \"#/components/schemas/RetryStrategy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-workflow-spec-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: WorkflowSpec
---
