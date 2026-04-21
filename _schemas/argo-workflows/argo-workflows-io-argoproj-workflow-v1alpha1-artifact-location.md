---
description: ArtifactLocation describes a location for a single or multiple artifacts. It is used as single artifact in the context of inputs/outputs (e.g. outputs.artifacts.artname). It is also used to describe the location of multiple artifacts such as the archive location of a single workflow step, which the executor will use as a default location to store its files.
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactLocation
properties_list:
- description: ArchiveLogs indicates if the container logs should be archived
  name: archiveLogs
  type: boolean
- description: Artifactory contains artifactory artifact location details
  name: artifactory
  type: object
- description: Azure contains Azure Storage artifact location details
  name: azure
  type: object
- description: GCS contains GCS artifact location details
  name: gcs
  type: object
- description: Git contains git artifact location details
  name: git
  type: object
- description: HDFS contains HDFS artifact location details
  name: hdfs
  type: object
- description: HTTP contains HTTP artifact location details
  name: http
  type: object
- description: OSS contains OSS artifact location details
  name: oss
  type: object
- description: Plugin contains plugin artifact location details
  name: plugin
  type: object
- description: Raw contains raw artifact location details
  name: raw
  type: object
- description: S3 contains S3 artifact location details
  name: s3
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-location-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifact-location
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactLocation
---
