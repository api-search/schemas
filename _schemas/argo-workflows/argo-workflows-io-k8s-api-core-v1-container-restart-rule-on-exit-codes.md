---
description: ContainerRestartRuleOnExitCodes describes the condition for handling an exited container based on its exit codes.
layout: schema
name: io.k8s.api.core.v1.ContainerRestartRuleOnExitCodes
properties_list:
- description: 'Represents the relationship between the container exit code(s) and the specified values. Possible values are: - In: the requirement is satisfied if the container exit code is in the set of specified v'
  name: operator
  type: string
- description: Specifies the set of values to check for container exit codes. At most 255 elements are allowed.
  name: values
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-container-restart-rule-on-exit-codes-schema.json
slug: argo-workflows-io-k8s-api-core-v1-container-restart-rule-on-exit-codes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-container-restart-rule-on-exit-codes-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ContainerRestartRuleOnExitCodes\",\n  \"description\": \"ContainerRestartRuleOnExitCodes describes the condition for handling an exited container based on its exit codes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operator\": {\n      \"description\": \"Represents the relationship between the container exit code(s) and the specified values. Possible values are: - In: the requirement is satisfied if the container exit code is in the\\n  set of specified values.\\n- NotIn: the requirement is satisfied if the container exit code is\\n  not in the set of specified values.\",\n      \"type\": \"string\"\n    },\n    \"values\": {\n      \"description\": \"Specifies the set of\
  \ values to check for container exit codes. At most 255 elements are allowed.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int32\"\n      },\n      \"x-kubernetes-list-type\": \"set\"\n    }\n  },\n  \"required\": [\n    \"operator\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-container-restart-rule-on-exit-codes-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ContainerRestartRuleOnExitCodes
---
