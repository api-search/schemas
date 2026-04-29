---
description: ContainerResizePolicy represents resource resize policy for the container.
layout: schema
name: io.k8s.api.core.v1.ContainerResizePolicy
properties_list:
- description: 'Name of the resource to which this resource resize policy applies. Supported values: cpu, memory.'
  name: resourceName
  type: string
- description: Restart policy to apply when specified resource is resized. If not specified, it defaults to NotRequired.
  name: restartPolicy
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-container-resize-policy-schema.json
slug: argo-workflows-io-k8s-api-core-v1-container-resize-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-container-resize-policy-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ContainerResizePolicy\",\n  \"description\": \"ContainerResizePolicy represents resource resize policy for the container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceName\": {\n      \"description\": \"Name of the resource to which this resource resize policy applies. Supported values: cpu, memory.\",\n      \"type\": \"string\"\n    },\n    \"restartPolicy\": {\n      \"description\": \"Restart policy to apply when specified resource is resized. If not specified, it defaults to NotRequired.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"resourceName\",\n    \"restartPolicy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-container-resize-policy-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ContainerResizePolicy
---
