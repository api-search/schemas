---
description: ArtifactoryArtifactRepository defines the controller configuration for an artifactory artifact repository
layout: schema
name: io.argoproj.workflow.v1alpha1.ArtifactoryArtifactRepository
properties_list:
- description: KeyFormat defines the format of how to store keys and can reference workflow variables.
  name: keyFormat
  type: string
- description: PasswordSecret is the secret selector to the repository password
  name: passwordSecret
  type: object
- description: RepoURL is the url for artifactory repo.
  name: repoURL
  type: string
- description: UsernameSecret is the secret selector to the repository username
  name: usernameSecret
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-repository-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-repository
source_filename: argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-repository-schema.json\",\n  \"title\": \"io.argoproj.workflow.v1alpha1.ArtifactoryArtifactRepository\",\n  \"description\": \"ArtifactoryArtifactRepository defines the controller configuration for an artifactory artifact repository\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"keyFormat\": {\n      \"description\": \"KeyFormat defines the format of how to store keys and can reference workflow variables.\",\n      \"type\": \"string\"\n    },\n    \"passwordSecret\": {\n      \"description\": \"PasswordSecret is the secret selector to the repository password\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"repoURL\": {\n      \"description\": \"RepoURL is the url for artifactory repo.\",\n\
  \      \"type\": \"string\"\n    },\n    \"usernameSecret\": {\n      \"description\": \"UsernameSecret is the secret selector to the repository username\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-artifactory-artifact-repository-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.ArtifactoryArtifactRepository
---
