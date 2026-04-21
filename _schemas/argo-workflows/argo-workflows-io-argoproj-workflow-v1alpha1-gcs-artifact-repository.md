---
description: GCSArtifactRepository defines the controller configuration for a GCS artifact repository
layout: schema
name: io.argoproj.workflow.v1alpha1.GCSArtifactRepository
properties_list:
- description: Bucket is the name of the bucket
  name: bucket
  type: string
- description: KeyFormat defines the format of how to store keys and can reference workflow variables.
  name: keyFormat
  type: string
- description: ServiceAccountKeySecret is the secret selector to the bucket's service account key
  name: serviceAccountKeySecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-gcs-artifact-repository-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-gcs-artifact-repository
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.GCSArtifactRepository
---
