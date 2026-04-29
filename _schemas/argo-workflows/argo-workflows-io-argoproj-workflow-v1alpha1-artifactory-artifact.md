---
description: ArtifactoryArtifact is the location of an artifactory artifact
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactoryArtifact
properties_list:
- description: PasswordSecret is the secret selector to the repository password
  name: passwordSecret
  type: object
- description: URL of the artifact
  name: url
  type: string
- description: UsernameSecret is the secret selector to the repository username
  name: usernameSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ArtifactoryArtifact\",\n  \"description\": \"ArtifactoryArtifact is the location of an artifactory artifact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"passwordSecret\": {\n      \"description\": \"PasswordSecret is the secret selector to the repository password\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"url\": {\n      \"description\": \"URL of the artifact\",\n      \"type\": \"string\"\n    },\n    \"usernameSecret\": {\n      \"description\": \"UsernameSecret is the secret selector to the repository username\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  },\n  \"required\": [\n \
  \   \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactoryArtifact
---
