---
description: Artifact indicates an artifact to place at a specified path
layout: schema
name: io.argoproj.workflow.v1alpha1.Artifact
properties_list:
- description: Archive controls how the artifact will be saved to the artifact repository.
  name: archive
  type: object
- description: ArchiveLogs indicates if the container logs should be archived
  name: archiveLogs
  type: boolean
- description: ArtifactGC describes the strategy to use when to deleting an artifact from completed or deleted workflows
  name: artifactGC
  type: object
- description: Artifactory contains artifactory artifact location details
  name: artifactory
  type: object
- description: Azure contains Azure Storage artifact location details
  name: azure
  type: object
- description: Has this been deleted?
  name: deleted
  type: boolean
- description: From allows an artifact to reference an artifact from a previous step
  name: from
  type: string
- description: FromExpression, if defined, is evaluated to specify the value for the artifact
  name: fromExpression
  type: string
- description: GCS contains GCS artifact location details
  name: gcs
  type: object
- description: Git contains git artifact location details
  name: git
  type: object
- description: GlobalName exports an output artifact to the global scope, making it available as '{{io.argoproj.workflow.v1alpha1.outputs.artifacts.XXXX}} and in workflow.status.outputs.artifacts
  name: globalName
  type: string
- description: HDFS contains HDFS artifact location details
  name: hdfs
  type: object
- description: HTTP contains HTTP artifact location details
  name: http
  type: object
- description: mode bits to use on this file, must be a value between 0 and 0777. Set when loading input artifacts. It is recommended to set the mode value to ensure the artifact has the expected permissions in your
  name: mode
  type: integer
- description: name of the artifact. must be unique within a template's inputs/outputs.
  name: name
  type: string
- description: Make Artifacts optional, if Artifacts doesn't generate or exist
  name: optional
  type: boolean
- description: OSS contains OSS artifact location details
  name: oss
  type: object
- description: Path is the container path to the artifact
  name: path
  type: string
- description: Plugin contains plugin artifact location details
  name: plugin
  type: object
- description: Raw contains raw artifact location details
  name: raw
  type: object
- description: If mode is set, apply the permission recursively into the artifact if it is a folder
  name: recurseMode
  type: boolean
- description: S3 contains S3 artifact location details
  name: s3
  type: object
- description: SubPath allows an artifact to be sourced from a subpath within the specified source
  name: subPath
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifact
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.Artifact
---
