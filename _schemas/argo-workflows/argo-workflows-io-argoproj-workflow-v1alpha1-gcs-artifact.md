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
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-gcs-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-gcs-artifact-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.GCSArtifact\",\n  \"description\": \"GCSArtifact is the location of a GCS artifact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"description\": \"Bucket is the name of the bucket\",\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"description\": \"Key is the path in the bucket where the artifact resides\",\n      \"type\": \"string\"\n    },\n    \"serviceAccountKeySecret\": {\n      \"description\": \"ServiceAccountKeySecret is the secret selector to the bucket's service account key\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  },\n  \"required\": [\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-gcs-artifact-schema.json
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
