---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.S3Artifact schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.S3Artifact
properties_list:
- description: ''
  name: accessKey
  type: object
- description: ''
  name: bucket
  type: object
- description: ''
  name: caCertificate
  type: object
- description: ''
  name: endpoint
  type: string
- description: ''
  name: events
  type: array
- description: ''
  name: filter
  type: object
- description: ''
  name: insecure
  type: boolean
- description: ''
  name: metadata
  type: object
- description: ''
  name: region
  type: string
- description: ''
  name: secretKey
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-s3-artifact-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-s3-artifact
source_filename: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-s3-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-s3-artifact-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.S3Artifact\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.S3Artifact schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessKey\": {\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"bucket\": {\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.S3Bucket\"\n    },\n    \"caCertificate\": {\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"endpoint\": {\n      \"type\": \"string\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"items\":\
  \ {\n        \"type\": \"string\"\n      }\n    },\n    \"filter\": {\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.S3Filter\"\n    },\n    \"insecure\": {\n      \"type\": \"boolean\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"region\": {\n      \"type\": \"string\"\n    },\n    \"secretKey\": {\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-s3-artifact-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.S3Artifact
---
