---
description: SubmitOpts are workflow submission options
layout: schema
name: io.argoproj.workflow.v1alpha1.SubmitOpts
properties_list:
- description: Annotations adds to metadata.labels
  name: annotations
  type: string
- description: DryRun validates the workflow on the client-side without creating it. This option is not supported in API
  name: dryRun
  type: boolean
- description: Entrypoint overrides spec.entrypoint
  name: entryPoint
  type: string
- description: GenerateName overrides metadata.generateName
  name: generateName
  type: string
- description: Labels adds to metadata.labels
  name: labels
  type: string
- description: Name overrides metadata.name
  name: name
  type: string
- description: OwnerReference creates a metadata.ownerReference
  name: ownerReference
  type: object
- description: Parameters passes input parameters to workflow
  name: parameters
  type: array
- description: Set the podPriorityClassName of the workflow
  name: podPriorityClassName
  type: string
- description: Priority is used if controller is configured to process limited number of workflows in parallel, higher priority workflows are processed first.
  name: priority
  type: integer
- description: ServerDryRun validates the workflow on the server-side without creating it
  name: serverDryRun
  type: boolean
- description: ServiceAccount runs all pods in the workflow using specified ServiceAccount.
  name: serviceAccount
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-submit-opts-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-submit-opts
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-submit-opts-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-submit-opts-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.SubmitOpts\",\n  \"description\": \"SubmitOpts are workflow submission options\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"annotations\": {\n      \"description\": \"Annotations adds to metadata.labels\",\n      \"type\": \"string\"\n    },\n    \"dryRun\": {\n      \"description\": \"DryRun validates the workflow on the client-side without creating it. This option is not supported in API\",\n      \"type\": \"boolean\"\n    },\n    \"entryPoint\": {\n      \"description\": \"Entrypoint overrides spec.entrypoint\",\n      \"type\": \"string\"\n    },\n    \"generateName\": {\n      \"description\": \"GenerateName overrides metadata.generateName\",\n      \"type\": \"string\"\n\
  \    },\n    \"labels\": {\n      \"description\": \"Labels adds to metadata.labels\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name overrides metadata.name\",\n      \"type\": \"string\"\n    },\n    \"ownerReference\": {\n      \"description\": \"OwnerReference creates a metadata.ownerReference\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.OwnerReference\"\n    },\n    \"parameters\": {\n      \"description\": \"Parameters passes input parameters to workflow\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"podPriorityClassName\": {\n      \"description\": \"Set the podPriorityClassName of the workflow\",\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"description\": \"Priority is used if controller is configured to process limited number of workflows in parallel, higher priority workflows are processed first.\",\n      \"type\": \"integer\"\n    },\n\
  \    \"serverDryRun\": {\n      \"description\": \"ServerDryRun validates the workflow on the server-side without creating it\",\n      \"type\": \"boolean\"\n    },\n    \"serviceAccount\": {\n      \"description\": \"ServiceAccount runs all pods in the workflow using specified ServiceAccount.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-submit-opts-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.SubmitOpts
---
