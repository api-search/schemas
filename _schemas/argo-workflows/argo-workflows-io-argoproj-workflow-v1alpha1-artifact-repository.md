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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ArtifactRepository\",\n  \"description\": \"ArtifactRepository represents an artifact repository in which a controller will store its artifacts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"archiveLogs\": {\n      \"description\": \"ArchiveLogs enables log archiving\",\n      \"type\": \"boolean\"\n    },\n    \"artifactory\": {\n      \"description\": \"Artifactory stores artifacts to JFrog Artifactory\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ArtifactoryArtifactRepository\"\n    },\n    \"azure\": {\n      \"description\": \"Azure stores artifact in an Azure Storage account\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.AzureArtifactRepository\"\
  \n    },\n    \"gcs\": {\n      \"description\": \"GCS stores artifact in a GCS object store\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.GCSArtifactRepository\"\n    },\n    \"hdfs\": {\n      \"description\": \"HDFS stores artifacts in HDFS\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.HDFSArtifactRepository\"\n    },\n    \"oss\": {\n      \"description\": \"OSS stores artifact in a OSS-compliant object store\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.OSSArtifactRepository\"\n    },\n    \"plugin\": {\n      \"description\": \"Plugin stores artifact in a plugin-specific artifact repository\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.PluginArtifactRepository\"\n    },\n    \"s3\": {\n      \"description\": \"S3 stores artifact in a S3-compliant object store\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.S3ArtifactRepository\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-repository-schema.json
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
