---
description: Maps a string key to a path within a volume.
layout: schema
name: io.k8s.api.core.v1.KeyToPath
properties_list:
- description: key is the key to project.
  name: key
  type: string
- description: 'mode is Optional: mode bits used to set permissions on this file. Must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and decimal values, JSON re'
  name: mode
  type: integer
- description: path is the relative path of the file to map the key to. May not be an absolute path. May not contain the path element '..'. May not start with the string '..'.
  name: path
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-key-to-path-schema.json
slug: argo-workflows-io-k8s-api-core-v1-key-to-path
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.KeyToPath
---
