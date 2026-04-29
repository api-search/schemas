---
description: ContainerRestartRule describes how a container exit is handled.
layout: schema
name: io.k8s.api.core.v1.ContainerRestartRule
properties_list:
- description: Specifies the action taken on a container exit if the requirements are satisfied. The only possible value is "Restart" to restart the container.
  name: action
  type: string
- description: Represents the exit codes to check on container exits.
  name: exitCodes
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-container-restart-rule-schema.json
slug: argo-workflows-io-k8s-api-core-v1-container-restart-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-container-restart-rule-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ContainerRestartRule\",\n  \"description\": \"ContainerRestartRule describes how a container exit is handled.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"description\": \"Specifies the action taken on a container exit if the requirements are satisfied. The only possible value is \\\"Restart\\\" to restart the container.\",\n      \"type\": \"string\"\n    },\n    \"exitCodes\": {\n      \"description\": \"Represents the exit codes to check on container exits.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ContainerRestartRuleOnExitCodes\"\n    }\n  },\n  \"required\": [\n    \"action\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-container-restart-rule-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ContainerRestartRule
---
