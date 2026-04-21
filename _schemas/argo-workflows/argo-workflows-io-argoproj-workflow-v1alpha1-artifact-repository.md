---
description: ArtifactRepository represents an artifact repository in which a controller will store its artifacts
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactRepository
properties_list:
- description: ArchiveLogs enables log archiving
  name: archiveLogs
  type: boolean
- description: Artifactory stores artifacts to JFrog Artifactory
  name: artifactory
  type: object
- description: Azure stores artifact in an Azure Storage account
  name: azure
  type: object
- description: GCS stores artifact in a GCS object store
  name: gcs
  type: object
- description: HDFS stores artifacts in HDFS
  name: hdfs
  type: object
- description: OSS stores artifact in a OSS-compliant object store
  name: oss
  type: object
- description: Plugin stores artifact in a plugin-specific artifact repository
  name: plugin
  type: object
- description: S3 stores artifact in a S3-compliant object store
  name: s3
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactRepository
---
