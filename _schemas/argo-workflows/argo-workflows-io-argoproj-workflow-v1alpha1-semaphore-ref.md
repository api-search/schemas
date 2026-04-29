---
description: SemaphoreRef is a reference of Semaphore
layout: schema
name: io.argoproj.workflow.v1alpha1.SemaphoreRef
properties_list:
- description: ConfigMapKeyRef is a configmap selector for Semaphore configuration
  name: configMapKeyRef
  type: object
- description: SyncDatabaseRef is a database reference for Semaphore configuration
  name: database
  type: object
- description: 'Namespace is the namespace of the configmap, default: [namespace of workflow]'
  name: namespace
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-ref-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-ref
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-ref-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.SemaphoreRef\",\n  \"description\": \"SemaphoreRef is a reference of Semaphore\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configMapKeyRef\": {\n      \"description\": \"ConfigMapKeyRef is a configmap selector for Semaphore configuration\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ConfigMapKeySelector\"\n    },\n    \"database\": {\n      \"description\": \"SyncDatabaseRef is a database reference for Semaphore configuration\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.SyncDatabaseRef\"\n    },\n    \"namespace\": {\n      \"description\": \"Namespace is the namespace of the configmap, default: [namespace of workflow]\",\n      \"type\": \"string\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-semaphore-ref-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.SemaphoreRef
---
