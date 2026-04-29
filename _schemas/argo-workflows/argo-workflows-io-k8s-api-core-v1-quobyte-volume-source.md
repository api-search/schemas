---
description: Represents a Quobyte mount that lasts the lifetime of a pod. Quobyte volumes do not support ownership management or SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.QuobyteVolumeSource
properties_list:
- description: group to map volume access to Default is no group
  name: group
  type: string
- description: readOnly here will force the Quobyte volume to be mounted with read-only permissions. Defaults to false.
  name: readOnly
  type: boolean
- description: registry represents a single or multiple Quobyte Registry services specified as a string as host:port pair (multiple entries are separated with commas) which acts as the central registry for volumes
  name: registry
  type: string
- description: tenant owning the given Quobyte volume in the Backend Used with dynamically provisioned Quobyte volumes, value is set by the plugin
  name: tenant
  type: string
- description: user to map volume access to Defaults to serivceaccount user
  name: user
  type: string
- description: volume is a string that references an already created Quobyte volume by name.
  name: volume
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-quobyte-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-quobyte-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-quobyte-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.QuobyteVolumeSource\",\n  \"description\": \"Represents a Quobyte mount that lasts the lifetime of a pod. Quobyte volumes do not support ownership management or SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"group\": {\n      \"description\": \"group to map volume access to Default is no group\",\n      \"type\": \"string\"\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly here will force the Quobyte volume to be mounted with read-only permissions. Defaults to false.\",\n      \"type\": \"boolean\"\n    },\n    \"registry\": {\n      \"description\": \"registry represents a single or multiple Quobyte Registry services specified as a string as host:port pair\
  \ (multiple entries are separated with commas) which acts as the central registry for volumes\",\n      \"type\": \"string\"\n    },\n    \"tenant\": {\n      \"description\": \"tenant owning the given Quobyte volume in the Backend Used with dynamically provisioned Quobyte volumes, value is set by the plugin\",\n      \"type\": \"string\"\n    },\n    \"user\": {\n      \"description\": \"user to map volume access to Defaults to serivceaccount user\",\n      \"type\": \"string\"\n    },\n    \"volume\": {\n      \"description\": \"volume is a string that references an already created Quobyte volume by name.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"registry\",\n    \"volume\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-quobyte-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.QuobyteVolumeSource
---
