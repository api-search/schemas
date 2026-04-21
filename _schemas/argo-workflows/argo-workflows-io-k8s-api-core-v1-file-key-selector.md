---
description: FileKeySelector selects a key of the env file.
layout: schema
name: io.k8s.api.core.v1.FileKeySelector
properties_list:
- description: The key within the env file. An invalid key will prevent the pod from starting. The keys defined within a source may consist of any printable ASCII characters except '='. During Alpha stage of the Env
  name: key
  type: string
- description: Specify whether the file or its key must be defined. If the file or key does not exist, then the env var is not published. If optional is set to true and the specified key does not exist, the environm
  name: optional
  type: boolean
- description: The path within the volume from which to select the file. Must be relative and may not contain the '..' path or start with '..'.
  name: path
  type: string
- description: The name of the volume mount containing the env file.
  name: volumeName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-file-key-selector-schema.json
slug: argo-workflows-io-k8s-api-core-v1-file-key-selector
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.FileKeySelector
---
