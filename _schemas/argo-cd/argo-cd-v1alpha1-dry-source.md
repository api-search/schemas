---
description: DrySource specifies a location for dry "don't repeat yourself" manifest source information.
layout: schema
name: v1alpha1DrySource
properties_list:
- description: ''
  name: directory
  type: object
- description: ''
  name: helm
  type: object
- description: ''
  name: kustomize
  type: object
- description: ''
  name: path
  type: string
- description: ''
  name: plugin
  type: object
- description: ''
  name: repoURL
  type: string
- description: ''
  name: targetRevision
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-dry-source-schema.json
slug: argo-cd-v1alpha1-dry-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-dry-source-schema.json\",\n  \"title\": \"v1alpha1DrySource\",\n  \"description\": \"DrySource specifies a location for dry \\\"don't repeat yourself\\\" manifest source information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directory\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSourceDirectory\"\n    },\n    \"helm\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSourceHelm\"\n    },\n    \"kustomize\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSourceKustomize\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"title\": \"Path is a directory path within the Git repository where the manifests are located\"\n    },\n    \"plugin\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSourcePlugin\"\n    },\n    \"repoURL\": {\n      \"\
  type\": \"string\",\n      \"title\": \"RepoURL is the URL to the git repository that contains the application manifests\"\n    },\n    \"targetRevision\": {\n      \"type\": \"string\",\n      \"title\": \"TargetRevision defines the revision of the source to hydrate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-dry-source-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1DrySource
---
