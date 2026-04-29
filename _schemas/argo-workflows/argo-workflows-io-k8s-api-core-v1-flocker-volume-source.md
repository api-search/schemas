---
description: Represents a Flocker volume mounted by the Flocker agent. One and only one of datasetName and datasetUUID should be set. Flocker volumes do not support ownership management or SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.FlockerVolumeSource
properties_list:
- description: datasetName is Name of the dataset stored as metadata -> name on the dataset for Flocker should be considered as deprecated
  name: datasetName
  type: string
- description: datasetUUID is the UUID of the dataset. This is unique identifier of a Flocker dataset
  name: datasetUUID
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-flocker-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-flocker-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-flocker-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.FlockerVolumeSource\",\n  \"description\": \"Represents a Flocker volume mounted by the Flocker agent. One and only one of datasetName and datasetUUID should be set. Flocker volumes do not support ownership management or SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"datasetName\": {\n      \"description\": \"datasetName is Name of the dataset stored as metadata -> name on the dataset for Flocker should be considered as deprecated\",\n      \"type\": \"string\"\n    },\n    \"datasetUUID\": {\n      \"description\": \"datasetUUID is the UUID of the dataset. This is unique identifier of a Flocker dataset\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-flocker-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.FlockerVolumeSource
---
