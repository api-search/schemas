---
description: Adapts a Secret into a volume. The contents of the target Secret's Data field will be presented in a volume as files using the keys in the Data field as the file names. Secret volumes support ownership management and SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.SecretVolumeSource
properties_list:
- description: 'defaultMode is Optional: mode bits used to set permissions on created files by default. Must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and d'
  name: defaultMode
  type: integer
- description: items If unspecified, each key-value pair in the Data field of the referenced Secret will be projected into the volume as a file whose name is the key and content is the value. If specified, the liste
  name: items
  type: array
- description: optional field specify whether the Secret or its keys must be defined
  name: optional
  type: boolean
- description: 'secretName is the name of the secret in the pod''s namespace to use. More info: https://kubernetes.io/docs/concepts/storage/volumes#secret'
  name: secretName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-secret-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-secret-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.SecretVolumeSource
---
