---
description: 'Represents a volume that is populated with the contents of a git repository. Git repo volumes do not support ownership management. Git repo volumes support SELinux relabeling. DEPRECATED: GitRepo is deprecated. To provision a container with a git repo, mount an EmptyDir into an InitContainer that clones the repo using git, then mount the EmptyDir into the Pod''s container.'
layout: schema
name: io.k8s.api.core.v1.GitRepoVolumeSource
properties_list:
- description: directory is the target directory name. Must not contain or start with '..'. If '.' is supplied, the volume directory will be the git repository. Otherwise, if specified, the volume will contain the g
  name: directory
  type: string
- description: repository is the URL
  name: repository
  type: string
- description: revision is the commit hash for the specified revision.
  name: revision
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-git-repo-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-git-repo-volume-source
source_filename: argo-workflows-io-k8s-api-core-v1-git-repo-volume-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-git-repo-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.GitRepoVolumeSource\",\n  \"description\": \"Represents a volume that is populated with the contents of a git repository. Git repo volumes do not support ownership management. Git repo volumes support SELinux relabeling.\\n\\nDEPRECATED: GitRepo is deprecated. To provision a container with a git repo, mount an EmptyDir into an InitContainer that clones the repo using git, then mount the EmptyDir into the Pod's container.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"directory\": {\n      \"description\": \"directory is the target directory name. Must not contain or start with '..'.  If '.' is supplied, the volume directory will be the git repository.  Otherwise, if specified, the volume will\
  \ contain the git repository in the subdirectory with the given name.\",\n      \"type\": \"string\"\n    },\n    \"repository\": {\n      \"description\": \"repository is the URL\",\n      \"type\": \"string\"\n    },\n    \"revision\": {\n      \"description\": \"revision is the commit hash for the specified revision.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"repository\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-git-repo-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.GitRepoVolumeSource
---
