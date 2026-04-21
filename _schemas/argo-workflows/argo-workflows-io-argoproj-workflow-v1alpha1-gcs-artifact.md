---
description: GCSArtifact is the location of a GCS artifact
layout: schema
name: io.argoproj.workflow.v1alpha1.GCSArtifact
properties_list:
- description: Bucket is the name of the bucket
  name: bucket
  type: string
- description: Key is the path in the bucket where the artifact resides
  name: key
  type: string
- description: ServiceAccountKeySecret is the secret selector to the bucket's service account key
  name: serviceAccountKeySecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-gcs-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-gcs-artifact
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.GCSArtifact
---
