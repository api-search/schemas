---
description: ResourceTemplate is a template subtype to manipulate kubernetes resources
layout: schema
name: io.argoproj.workflow.v1alpha1.ResourceTemplate
properties_list:
- description: 'Action is the action to perform to the resource. Must be one of: get, create, apply, delete, replace, patch'
  name: action
  type: string
- description: FailureCondition is a label selector expression which describes the conditions of the k8s resource in which the step was considered failed
  name: failureCondition
  type: string
- description: 'Flags is a set of additional options passed to kubectl before submitting a resource I.e. to disable resource validation: flags: [ "--validate=false" # disable resource validation ]'
  name: flags
  type: array
- description: Manifest contains the kubernetes manifest
  name: manifest
  type: string
- description: ManifestFrom is the source for a single kubernetes manifest
  name: manifestFrom
  type: object
- description: 'MergeStrategy is the strategy used to merge a patch. It defaults to "strategic" Must be one of: strategic, merge, json'
  name: mergeStrategy
  type: string
- description: SetOwnerReference sets the reference to the workflow on the OwnerReference of generated resource.
  name: setOwnerReference
  type: boolean
- description: SuccessCondition is a label selector expression which describes the conditions of the k8s resource in which it is acceptable to proceed to the following step
  name: successCondition
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-resource-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-resource-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-resource-template-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ResourceTemplate\",\n  \"description\": \"ResourceTemplate is a template subtype to manipulate kubernetes resources\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"description\": \"Action is the action to perform to the resource. Must be one of: get, create, apply, delete, replace, patch\",\n      \"type\": \"string\"\n    },\n    \"failureCondition\": {\n      \"description\": \"FailureCondition is a label selector expression which describes the conditions of the k8s resource in which the step was considered failed\",\n      \"type\": \"string\"\n    },\n    \"flags\": {\n      \"description\": \"Flags is a set of additional options passed to kubectl before\
  \ submitting a resource I.e. to disable resource validation: flags: [\\n\\t\\\"--validate=false\\\"  # disable resource validation\\n]\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"manifest\": {\n      \"description\": \"Manifest contains the kubernetes manifest\",\n      \"type\": \"string\"\n    },\n    \"manifestFrom\": {\n      \"description\": \"ManifestFrom is the source for a single kubernetes manifest\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ManifestFrom\"\n    },\n    \"mergeStrategy\": {\n      \"description\": \"MergeStrategy is the strategy used to merge a patch. It defaults to \\\"strategic\\\" Must be one of: strategic, merge, json\",\n      \"type\": \"string\"\n    },\n    \"setOwnerReference\": {\n      \"description\": \"SetOwnerReference sets the reference to the workflow on the OwnerReference of generated resource.\",\n      \"type\": \"boolean\"\n    },\n    \"successCondition\": {\n\
  \      \"description\": \"SuccessCondition is a label selector expression which describes the conditions of the k8s resource in which it is acceptable to proceed to the following step\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-resource-template-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ResourceTemplate
---
