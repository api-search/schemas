---
description: Represents a volume that is populated with the contents of a git repository
layout: schema
name: GitRepoVolume
properties_list:
- description: 'Target directory name. Must not contain or start with ''..''. If ''.'' is supplied, the volume directory will be the git repository. Otherwise, if specified, the volume will contain the git repository in '
  name: directory
  type: string
- description: Repository URL
  name: repository
  type: string
- description: Commit hash for the specified revision.
  name: revision
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-git-repo-volume-schema.json
slug: azure-container-instances-git-repo-volume
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: GitRepoVolume
---
