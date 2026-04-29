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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-key-to-path-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.KeyToPath\",\n  \"description\": \"Maps a string key to a path within a volume.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"description\": \"key is the key to project.\",\n      \"type\": \"string\"\n    },\n    \"mode\": {\n      \"description\": \"mode is Optional: mode bits used to set permissions on this file. Must be an octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML accepts both octal and decimal values, JSON requires decimal values for mode bits. If not specified, the volume defaultMode will be used. This might be in conflict with other options that affect the file mode, like fsGroup, and the result can be other mode bits set.\",\n      \"type\"\
  : \"integer\"\n    },\n    \"path\": {\n      \"description\": \"path is the relative path of the file to map the key to. May not be an absolute path. May not contain the path element '..'. May not start with the string '..'.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-key-to-path-schema.json
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
