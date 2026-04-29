---
description: The pod this Toleration is attached to tolerates any taint that matches the triple <key,value,effect> using the matching operator <operator>.
layout: schema
name: io.k8s.api.core.v1.Toleration
properties_list:
- description: Effect indicates the taint effect to match. Empty means match all taint effects. When specified, allowed values are NoSchedule, PreferNoSchedule and NoExecute.
  name: effect
  type: string
- description: Key is the taint key that the toleration applies to. Empty means match all taint keys. If the key is empty, operator must be Exists; this combination means to match all values and all keys.
  name: key
  type: string
- description: Operator represents a key's relationship to the value. Valid operators are Exists, Equal, Lt, and Gt. Defaults to Equal. Exists is equivalent to wildcard for value, so that a pod can tolerate all tain
  name: operator
  type: string
- description: TolerationSeconds represents the period of time the toleration (which must be of effect NoExecute, otherwise this field is ignored) tolerates the taint. By default, it is not set, which means tolerate
  name: tolerationSeconds
  type: integer
- description: Value is the taint value the toleration matches to. If the operator is Exists, the value should be empty, otherwise just a regular string.
  name: value
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-toleration-schema.json
slug: argo-workflows-io-k8s-api-core-v1-toleration
source_filename: argo-workflows-io-k8s-api-core-v1-toleration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-toleration-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.Toleration\",\n  \"description\": \"The pod this Toleration is attached to tolerates any taint that matches the triple <key,value,effect> using the matching operator <operator>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"effect\": {\n      \"description\": \"Effect indicates the taint effect to match. Empty means match all taint effects. When specified, allowed values are NoSchedule, PreferNoSchedule and NoExecute.\",\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"description\": \"Key is the taint key that the toleration applies to. Empty means match all taint keys. If the key is empty, operator must be Exists; this combination means to match all values and all keys.\",\n      \"type\"\
  : \"string\"\n    },\n    \"operator\": {\n      \"description\": \"Operator represents a key's relationship to the value. Valid operators are Exists, Equal, Lt, and Gt. Defaults to Equal. Exists is equivalent to wildcard for value, so that a pod can tolerate all taints of a particular category. Lt and Gt perform numeric comparisons (requires feature gate TaintTolerationComparisonOperators).\",\n      \"type\": \"string\"\n    },\n    \"tolerationSeconds\": {\n      \"description\": \"TolerationSeconds represents the period of time the toleration (which must be of effect NoExecute, otherwise this field is ignored) tolerates the taint. By default, it is not set, which means tolerate the taint forever (do not evict). Zero and negative values will be treated as 0 (evict immediately) by the system.\",\n      \"type\": \"integer\"\n    },\n    \"value\": {\n      \"description\": \"Value is the taint value the toleration matches to. If the operator is Exists, the value should be empty, otherwise\
  \ just a regular string.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-toleration-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.Toleration
---
