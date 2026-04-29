---
description: PersistentVolumeClaimCondition contains details about state of pvc
layout: schema
name: io.k8s.api.core.v1.PersistentVolumeClaimCondition
properties_list:
- description: lastProbeTime is the time we probed the condition.
  name: lastProbeTime
  type: object
- description: lastTransitionTime is the time the condition transitioned from one status to another.
  name: lastTransitionTime
  type: object
- description: message is the human-readable message indicating details about last transition.
  name: message
  type: string
- description: reason is a unique, this should be a short, machine understandable string that gives the reason for condition's last transition. If it reports "Resizing" that means the underlying persistent volume is
  name: reason
  type: string
- description: 'Status is the status of the condition. Can be True, False, Unknown. More info: https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-claim-v1/#:~:text=stat'
  name: status
  type: string
- description: 'Type is the type of the condition. More info: https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-claim-v1/#:~:text=set%20to%20%27ResizeStarted%27.-,Pers'
  name: type
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-condition-schema.json
slug: argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-condition
source_filename: argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-condition-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PersistentVolumeClaimCondition\",\n  \"description\": \"PersistentVolumeClaimCondition contains details about state of pvc\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastProbeTime\": {\n      \"description\": \"lastProbeTime is the time we probed the condition.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"lastTransitionTime\": {\n      \"description\": \"lastTransitionTime is the time the condition transitioned from one status to another.\",\n      \"$ref\": \"#/definitions/io.k8s.apimachinery.pkg.apis.meta.v1.Time\"\n    },\n    \"message\": {\n      \"description\": \"message is the human-readable message indicating details\
  \ about last transition.\",\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"description\": \"reason is a unique, this should be a short, machine understandable string that gives the reason for condition's last transition. If it reports \\\"Resizing\\\" that means the underlying persistent volume is being resized.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"Status is the status of the condition. Can be True, False, Unknown. More info: https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-claim-v1/#:~:text=state%20of%20pvc-,conditions.status,-(string)%2C%20required\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"description\": \"Type is the type of the condition. More info: https://kubernetes.io/docs/reference/kubernetes-api/config-and-storage-resources/persistent-volume-claim-v1/#:~:text=set%20to%20%27ResizeStarted%27.-,PersistentVolumeClaimCondition,-contains%20details%20about\"\
  ,\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-condition-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PersistentVolumeClaimCondition
---
