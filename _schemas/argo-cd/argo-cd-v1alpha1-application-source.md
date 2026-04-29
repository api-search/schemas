---
description: v1alpha1ApplicationSource schema from Argo CD API
layout: schema
name: v1alpha1ApplicationSource
properties_list:
- description: Chart is a Helm chart name, and must be specified for applications sourced from a Helm repo.
  name: chart
  type: string
- description: ''
  name: directory
  type: object
- description: ''
  name: helm
  type: object
- description: ''
  name: kustomize
  type: object
- description: Name is used to refer to a source and is displayed in the UI. It is used in multi-source Applications.
  name: name
  type: string
- description: Path is a directory path within the Git repository, and is only valid for applications sourced from Git.
  name: path
  type: string
- description: ''
  name: plugin
  type: object
- description: Ref is reference to another source within sources field. This field will not be used if used with a `source` tag.
  name: ref
  type: string
- description: ''
  name: repoURL
  type: string
- description: 'TargetRevision defines the revision of the source to sync the application to. In case of Git, this can be commit, tag, or branch. If omitted, will equal to HEAD. In case of Helm, this is a semver tag '
  name: targetRevision
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-source-schema.json
slug: argo-cd-v1alpha1-application-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-schema.json\",\n  \"title\": \"v1alpha1ApplicationSource\",\n  \"description\": \"v1alpha1ApplicationSource schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"chart\": {\n      \"description\": \"Chart is a Helm chart name, and must be specified for applications sourced from a Helm repo.\",\n      \"type\": \"string\"\n    },\n    \"directory\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSourceDirectory\"\n    },\n    \"helm\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSourceHelm\"\n    },\n    \"kustomize\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSourceKustomize\"\n    },\n    \"name\": {\n      \"description\": \"Name is used to refer to a source and is displayed in the UI. It is used in multi-source Applications.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"path\": {\n      \"description\": \"Path is a directory path within the Git repository, and is only valid for applications sourced from Git.\",\n      \"type\": \"string\"\n    },\n    \"plugin\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSourcePlugin\"\n    },\n    \"ref\": {\n      \"description\": \"Ref is reference to another source within sources field. This field will not be used if used with a `source` tag.\",\n      \"type\": \"string\"\n    },\n    \"repoURL\": {\n      \"type\": \"string\",\n      \"title\": \"RepoURL is the URL to the repository (Git or Helm) that contains the application manifests\"\n    },\n    \"targetRevision\": {\n      \"description\": \"TargetRevision defines the revision of the source to sync the application to.\\nIn case of Git, this can be commit, tag, or branch. If omitted, will equal to HEAD.\\nIn case of Helm, this is a semver tag for the Chart's version.\",\n      \"type\": \"string\"\n \
  \   }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-source-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSource
---
