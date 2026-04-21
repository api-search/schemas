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
