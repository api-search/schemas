---
description: AzureFile represents an Azure File Service mount on the host and bind mount to the pod.
layout: schema
name: io.k8s.api.core.v1.AzureFileVolumeSource
properties_list:
- description: readOnly defaults to false (read/write). ReadOnly here will force the ReadOnly setting in VolumeMounts.
  name: readOnly
  type: boolean
- description: secretName is the name of secret that contains Azure Storage Account Name and Key
  name: secretName
  type: string
- description: shareName is the azure share Name
  name: shareName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-azure-file-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-azure-file-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.AzureFileVolumeSource
---
