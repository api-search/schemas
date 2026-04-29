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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-location-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ArtifactLocation\",\n  \"description\": \"ArtifactLocation describes a location for a single or multiple artifacts. It is used as single artifact in the context of inputs/outputs (e.g. outputs.artifacts.artname). It is also used to describe the location of multiple artifacts such as the archive location of a single workflow step, which the executor will use as a default location to store its files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"archiveLogs\": {\n      \"description\": \"ArchiveLogs indicates if the container logs should be archived\",\n      \"type\": \"boolean\"\n    },\n    \"artifactory\": {\n      \"description\": \"Artifactory contains artifactory artifact\
  \ location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ArtifactoryArtifact\"\n    },\n    \"azure\": {\n      \"description\": \"Azure contains Azure Storage artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.AzureArtifact\"\n    },\n    \"gcs\": {\n      \"description\": \"GCS contains GCS artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.GCSArtifact\"\n    },\n    \"git\": {\n      \"description\": \"Git contains git artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.GitArtifact\"\n    },\n    \"hdfs\": {\n      \"description\": \"HDFS contains HDFS artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.HDFSArtifact\"\n    },\n    \"http\": {\n      \"description\": \"HTTP contains HTTP artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.HTTPArtifact\"\n  \
  \  },\n    \"oss\": {\n      \"description\": \"OSS contains OSS artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.OSSArtifact\"\n    },\n    \"plugin\": {\n      \"description\": \"Plugin contains plugin artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.PluginArtifact\"\n    },\n    \"raw\": {\n      \"description\": \"Raw contains raw artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.RawArtifact\"\n    },\n    \"s3\": {\n      \"description\": \"S3 contains S3 artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.S3Artifact\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-location-schema.json
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
