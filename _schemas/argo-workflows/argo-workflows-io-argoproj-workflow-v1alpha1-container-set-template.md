---
description: io.argoproj.workflow.v1alpha1.ContainerSetTemplate schema from Argo Workflows API
layout: schema
name: io.argoproj.workflow.v1alpha1.ContainerSetTemplate
properties_list:
- description: ''
  name: containers
  type: array
- description: RetryStrategy describes how to retry container nodes if the container set fails. Note that this works differently from the template-level `retryStrategy` as it is a process-level retry that does not c
  name: retryStrategy
  type: object
- description: ''
  name: volumeMounts
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-container-set-template-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-container-set-template
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-container-set-template-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ContainerSetTemplate\",\n  \"description\": \"io.argoproj.workflow.v1alpha1.ContainerSetTemplate schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"containers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ContainerNode\"\n      }\n    },\n    \"retryStrategy\": {\n      \"description\": \"RetryStrategy describes how to retry container nodes if the container set fails. Note that this works differently from the template-level `retryStrategy` as it is a process-level retry that does not create new Pods or containers.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ContainerSetRetryStrategy\"\
  \n    },\n    \"volumeMounts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.VolumeMount\"\n      }\n    }\n  },\n  \"required\": [\n    \"containers\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-container-set-template-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ContainerSetTemplate
---
