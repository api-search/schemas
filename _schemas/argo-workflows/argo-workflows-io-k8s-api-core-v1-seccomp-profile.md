---
description: SeccompProfile defines a pod/container's seccomp profile settings. Only one profile source may be set.
layout: schema
name: io.k8s.api.core.v1.SeccompProfile
properties_list:
- description: localhostProfile indicates a profile defined in a file on the node should be used. The profile must be preconfigured on the node to work. Must be a descending path, relative to the kubelet's configure
  name: localhostProfile
  type: string
- description: 'type indicates which kind of seccomp profile will be applied. Valid options are: Localhost - a profile defined in a file on the node should be used. RuntimeDefault - the container runtime default prof'
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-seccomp-profile-schema.json
slug: argo-workflows-io-k8s-api-core-v1-seccomp-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-seccomp-profile-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.SeccompProfile\",\n  \"description\": \"SeccompProfile defines a pod/container's seccomp profile settings. Only one profile source may be set.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"localhostProfile\": {\n      \"description\": \"localhostProfile indicates a profile defined in a file on the node should be used. The profile must be preconfigured on the node to work. Must be a descending path, relative to the kubelet's configured seccomp profile location. Must be set if type is \\\"Localhost\\\". Must NOT be set for any other type.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"type indicates which kind of seccomp profile will be applied. Valid options are:\\\
  n\\nLocalhost - a profile defined in a file on the node should be used. RuntimeDefault - the container runtime default profile should be used. Unconfined - no profile should be applied.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-seccomp-profile-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.SeccompProfile
---
