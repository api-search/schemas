---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArtifactLocation schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArtifactLocation
properties_list:
- description: ''
  name: configmap
  type: object
- description: ''
  name: file
  type: object
- description: ''
  name: git
  type: object
- description: ''
  name: inline
  type: string
- description: ''
  name: resource
  type: object
- description: ''
  name: s3
  type: object
- description: ''
  name: url
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-artifact-location-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-artifact-location
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-artifact-location-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-artifact-location-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArtifactLocation\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArtifactLocation schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configmap\": {\n      \"title\": \"Configmap that stores the artifact\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ConfigMapKeySelector\"\n    },\n    \"file\": {\n      \"title\": \"File artifact is artifact stored in a file\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.FileArtifact\"\n    },\n    \"git\": {\n      \"title\": \"Git repository hosting the artifact\",\n    \
  \  \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.GitArtifact\"\n    },\n    \"inline\": {\n      \"type\": \"string\",\n      \"title\": \"Inline artifact is embedded in sensor spec as a string\"\n    },\n    \"resource\": {\n      \"title\": \"Resource is generic template for K8s resource\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.K8SResource\"\n    },\n    \"s3\": {\n      \"title\": \"S3 compliant artifact\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.S3Artifact\"\n    },\n    \"url\": {\n      \"title\": \"URL to fetch the artifact from\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.URLArtifact\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-artifact-location-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.ArtifactLocation
---
