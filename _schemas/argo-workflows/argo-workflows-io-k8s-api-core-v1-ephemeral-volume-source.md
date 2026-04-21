---
description: Represents an ephemeral volume that is handled by a normal storage driver.
layout: schema
name: io.k8s.api.core.v1.EphemeralVolumeSource
properties_list:
- description: Will be used to create a stand-alone PVC to provision the volume. The pod in which this EphemeralVolumeSource is embedded will be the owner of the PVC, i.e. the PVC will be deleted together with the p
  name: volumeClaimTemplate
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-ephemeral-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-ephemeral-volume-source
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.EphemeralVolumeSource
---
