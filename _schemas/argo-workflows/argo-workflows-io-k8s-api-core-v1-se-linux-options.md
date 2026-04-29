---
description: SELinuxOptions are the labels to be applied to the container
layout: schema
name: io.k8s.api.core.v1.SELinuxOptions
properties_list:
- description: Level is SELinux level label that applies to the container.
  name: level
  type: string
- description: Role is a SELinux role label that applies to the container.
  name: role
  type: string
- description: Type is a SELinux type label that applies to the container.
  name: type
  type: string
- description: User is a SELinux user label that applies to the container.
  name: user
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-se-linux-options-schema.json
slug: argo-workflows-io-k8s-api-core-v1-se-linux-options
source_filename: argo-workflows-io-k8s-api-core-v1-se-linux-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-se-linux-options-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.SELinuxOptions\",\n  \"description\": \"SELinuxOptions are the labels to be applied to the container\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"level\": {\n      \"description\": \"Level is SELinux level label that applies to the container.\",\n      \"type\": \"string\"\n    },\n    \"role\": {\n      \"description\": \"Role is a SELinux role label that applies to the container.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type is a SELinux type label that applies to the container.\",\n      \"type\": \"string\"\n    },\n    \"user\": {\n      \"description\": \"User is a SELinux user label that applies to the container.\",\n      \"type\": \"string\"\n\
  \    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-se-linux-options-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.SELinuxOptions
---
