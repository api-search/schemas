---
description: HydrateTo specifies a location to which hydrated manifests should be pushed as a "staging area" before being moved to the SyncSource. The RepoURL and Path are assumed based on the associated SyncSource config in the SourceHydrator.
layout: schema
name: v1alpha1HydrateTo
properties_list:
- description: ''
  name: targetBranch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-hydrate-to-schema.json
slug: argo-cd-v1alpha1-hydrate-to
source_filename: argo-cd-v1alpha1-hydrate-to-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-hydrate-to-schema.json\",\n  \"title\": \"v1alpha1HydrateTo\",\n  \"description\": \"HydrateTo specifies a location to which hydrated manifests should be pushed as a \\\"staging area\\\" before being moved to\\nthe SyncSource. The RepoURL and Path are assumed based on the associated SyncSource config in the SourceHydrator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetBranch\": {\n      \"type\": \"string\",\n      \"title\": \"TargetBranch is the branch to which hydrated manifests should be committed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-hydrate-to-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1HydrateTo
---
