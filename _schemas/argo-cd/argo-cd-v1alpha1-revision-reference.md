---
description: RevisionReference contains a reference to a some information that is related in some way to another commit. For now, it supports only references to a commit. In the future, it may support other types of references.
layout: schema
name: v1alpha1RevisionReference
properties_list:
- description: ''
  name: commit
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-revision-reference-schema.json
slug: argo-cd-v1alpha1-revision-reference
source_filename: argo-cd-v1alpha1-revision-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-revision-reference-schema.json\",\n  \"title\": \"v1alpha1RevisionReference\",\n  \"description\": \"RevisionReference contains a reference to a some information that is related in some way to another commit. For now,\\nit supports only references to a commit. In the future, it may support other types of references.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"commit\": {\n      \"$ref\": \"#/definitions/v1alpha1CommitMetadata\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-revision-reference-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1RevisionReference
---
