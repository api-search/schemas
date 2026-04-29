---
description: EnvVarSource represents a source for the value of an EnvVar.
layout: schema
name: io.k8s.api.core.v1.EnvVarSource
properties_list:
- description: Selects a key of a ConfigMap.
  name: configMapKeyRef
  type: object
- description: 'Selects a field of the pod: supports metadata.name, metadata.namespace, `metadata.labels[''<KEY>'']`, `metadata.annotations[''<KEY>'']`, spec.nodeName, spec.serviceAccountName, status.hostIP, status.podIP'
  name: fieldRef
  type: object
- description: FileKeyRef selects a key of the env file. Requires the EnvFiles feature gate to be enabled.
  name: fileKeyRef
  type: object
- description: 'Selects a resource of the container: only resources limits and requests (limits.cpu, limits.memory, limits.ephemeral-storage, requests.cpu, requests.memory and requests.ephemeral-storage) are currentl'
  name: resourceFieldRef
  type: object
- description: Selects a key of a secret in the pod's namespace
  name: secretKeyRef
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-env-var-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-env-var-source
source_filename: argo-workflows-io-k8s-api-core-v1-env-var-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-env-var-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.EnvVarSource\",\n  \"description\": \"EnvVarSource represents a source for the value of an EnvVar.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configMapKeyRef\": {\n      \"description\": \"Selects a key of a ConfigMap.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ConfigMapKeySelector\"\n    },\n    \"fieldRef\": {\n      \"description\": \"Selects a field of the pod: supports metadata.name, metadata.namespace, `metadata.labels['<KEY>']`, `metadata.annotations['<KEY>']`, spec.nodeName, spec.serviceAccountName, status.hostIP, status.podIP, status.podIPs.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ObjectFieldSelector\"\n    },\n    \"fileKeyRef\": {\n      \"description\": \"\
  FileKeyRef selects a key of the env file. Requires the EnvFiles feature gate to be enabled.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.FileKeySelector\"\n    },\n    \"resourceFieldRef\": {\n      \"description\": \"Selects a resource of the container: only resources limits and requests (limits.cpu, limits.memory, limits.ephemeral-storage, requests.cpu, requests.memory and requests.ephemeral-storage) are currently supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ResourceFieldSelector\"\n    },\n    \"secretKeyRef\": {\n      \"description\": \"Selects a key of a secret in the pod's namespace\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-env-var-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EnvVarSource
---
