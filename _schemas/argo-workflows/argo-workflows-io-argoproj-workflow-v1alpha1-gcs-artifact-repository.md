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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-gcs-artifact-repository-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.GCSArtifactRepository\",\n  \"description\": \"GCSArtifactRepository defines the controller configuration for a GCS artifact repository\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"description\": \"Bucket is the name of the bucket\",\n      \"type\": \"string\"\n    },\n    \"keyFormat\": {\n      \"description\": \"KeyFormat defines the format of how to store keys and can reference workflow variables.\",\n      \"type\": \"string\"\n    },\n    \"serviceAccountKeySecret\": {\n      \"description\": \"ServiceAccountKeySecret is the secret selector to the bucket's service account key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-gcs-artifact-repository-schema.json
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
