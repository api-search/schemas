---
description: PersistentVolumeClaimTemplate is used to produce PersistentVolumeClaim objects as part of an EphemeralVolumeSource.
layout: schema
name: io.k8s.api.core.v1.PersistentVolumeClaimTemplate
properties_list:
- description: May contain labels and annotations that will be copied into the PVC when creating it. No other fields are allowed and will be rejected during validation.
  name: metadata
  type: object
- description: 'The specification for the PersistentVolumeClaim. The entire content is copied unchanged into the PVC that gets created from this template. The same fields as in a PersistentVolumeClaim are also valid '
  name: spec
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-template-schema.json
slug: argo-workflows-io-k8s-api-core-v1-persistent-volume-claim-template
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PersistentVolumeClaimTemplate
---
