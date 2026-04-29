---
description: ArtifactPaths expands a step from a collection of artifacts
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactPaths
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
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-paths-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifact-paths
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-paths-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ArtifactPaths\",\n  \"description\": \"ArtifactPaths expands a step from a collection of artifacts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"archive\": {\n      \"description\": \"Archive controls how the artifact will be saved to the artifact repository.\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ArchiveStrategy\"\n    },\n    \"archiveLogs\": {\n      \"description\": \"ArchiveLogs indicates if the container logs should be archived\",\n      \"type\": \"boolean\"\n    },\n    \"artifactGC\": {\n      \"description\": \"ArtifactGC describes the strategy to use when to deleting an artifact from completed or deleted workflows\",\n      \"$ref\": \"\
  #/definitions/io.argoproj.workflow.v1alpha1.ArtifactGC\"\n    },\n    \"artifactory\": {\n      \"description\": \"Artifactory contains artifactory artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.ArtifactoryArtifact\"\n    },\n    \"azure\": {\n      \"description\": \"Azure contains Azure Storage artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.AzureArtifact\"\n    },\n    \"deleted\": {\n      \"description\": \"Has this been deleted?\",\n      \"type\": \"boolean\"\n    },\n    \"from\": {\n      \"description\": \"From allows an artifact to reference an artifact from a previous step\",\n      \"type\": \"string\"\n    },\n    \"fromExpression\": {\n      \"description\": \"FromExpression, if defined, is evaluated to specify the value for the artifact\",\n      \"type\": \"string\"\n    },\n    \"gcs\": {\n      \"description\": \"GCS contains GCS artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.GCSArtifact\"\
  \n    },\n    \"git\": {\n      \"description\": \"Git contains git artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.GitArtifact\"\n    },\n    \"globalName\": {\n      \"description\": \"GlobalName exports an output artifact to the global scope, making it available as '{{io.argoproj.workflow.v1alpha1.outputs.artifacts.XXXX}} and in workflow.status.outputs.artifacts\",\n      \"type\": \"string\"\n    },\n    \"hdfs\": {\n      \"description\": \"HDFS contains HDFS artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.HDFSArtifact\"\n    },\n    \"http\": {\n      \"description\": \"HTTP contains HTTP artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.HTTPArtifact\"\n    },\n    \"mode\": {\n      \"description\": \"mode bits to use on this file, must be a value between 0 and 0777. Set when loading input artifacts. It is recommended to set the mode value to ensure the\
  \ artifact has the expected permissions in your container.\",\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"description\": \"name of the artifact. must be unique within a template's inputs/outputs.\",\n      \"type\": \"string\"\n    },\n    \"optional\": {\n      \"description\": \"Make Artifacts optional, if Artifacts doesn't generate or exist\",\n      \"type\": \"boolean\"\n    },\n    \"oss\": {\n      \"description\": \"OSS contains OSS artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.OSSArtifact\"\n    },\n    \"path\": {\n      \"description\": \"Path is the container path to the artifact\",\n      \"type\": \"string\"\n    },\n    \"plugin\": {\n      \"description\": \"Plugin contains plugin artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.PluginArtifact\"\n    },\n    \"raw\": {\n      \"description\": \"Raw contains raw artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.RawArtifact\"\
  \n    },\n    \"recurseMode\": {\n      \"description\": \"If mode is set, apply the permission recursively into the artifact if it is a folder\",\n      \"type\": \"boolean\"\n    },\n    \"s3\": {\n      \"description\": \"S3 contains S3 artifact location details\",\n      \"$ref\": \"#/definitions/io.argoproj.workflow.v1alpha1.S3Artifact\"\n    },\n    \"subPath\": {\n      \"description\": \"SubPath allows an artifact to be sourced from a subpath within the specified source\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifact-paths-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactPaths
---
