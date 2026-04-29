---
description: SyncSource specifies a location from which hydrated manifests may be synced. RepoURL is assumed based on the associated DrySource config in the SourceHydrator.
layout: schema
name: v1alpha1SyncSource
properties_list:
- description: Path is a directory path within the git repository where hydrated manifests should be committed to and synced from. The Path should never point to the root of the repo. If hydrateTo is set, this is ju
  name: path
  type: string
- description: TargetBranch is the branch from which hydrated manifests will be synced. If HydrateTo is not set, this is also the branch to which hydrated manifests are committed.
  name: targetBranch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-sync-source-schema.json
slug: argo-cd-v1alpha1-sync-source
source_filename: argo-cd-v1alpha1-sync-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-source-schema.json\",\n  \"title\": \"v1alpha1SyncSource\",\n  \"description\": \"SyncSource specifies a location from which hydrated manifests may be synced. RepoURL is assumed based on the\\nassociated DrySource config in the SourceHydrator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"description\": \"Path is a directory path within the git repository where hydrated manifests should be committed to and synced\\nfrom. The Path should never point to the root of the repo. If hydrateTo is set, this is just the path from which\\nhydrated manifests will be synced.\\n\\n+kubebuilder:validation:Required\\n+kubebuilder:validation:MinLength=1\\n+kubebuilder:validation:Pattern=`^.{2,}|[^./]$`\",\n      \"type\": \"string\"\n    },\n    \"targetBranch\": {\n      \"description\"\
  : \"TargetBranch is the branch from which hydrated manifests will be synced.\\nIf HydrateTo is not set, this is also the branch to which hydrated manifests are committed.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-sync-source-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SyncSource
---
