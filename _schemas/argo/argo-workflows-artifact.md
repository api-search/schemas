---
description: A workflow artifact
layout: schema
name: Artifact
properties_list:
- description: ''
  name: name
  type: string
- description: Path in the container where artifact is placed
  name: path
  type: string
- description: Source artifact reference
  name: from
  type: string
- description: ''
  name: s3
  type: object
- description: ''
  name: git
  type: object
- description: ''
  name: http
  type: object
- description: ''
  name: archive
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-workflows-artifact-schema.json
slug: argo-workflows-artifact
source_filename: argo-workflows-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-artifact-schema.json\",\n  \"title\": \"Artifact\",\n  \"description\": \"A workflow artifact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Path in the container where artifact is placed\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"Source artifact reference\"\n    },\n    \"s3\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"bucket\": {\n          \"type\": \"string\"\n        },\n        \"key\": {\n          \"type\": \"string\"\n        },\n        \"endpoint\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"git\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"repo\": {\n\
  \          \"type\": \"string\"\n        },\n        \"revision\": {\n          \"type\": \"string\"\n        },\n        \"depth\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"http\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\"\n        },\n        \"headers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        }\n      }\n    },\n    \"archive\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"none\": {\n          \"type\": \"object\"\n        },\n        \"tar\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"compressionLevel\": {\n              \"type\": \"integer\"\n            }\n          }\n        },\n        \"zip\": {\n          \"type\": \"object\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-workflows-artifact-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Artifact
---
