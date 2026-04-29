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
source_filename: azure-container-instances-git-repo-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-git-repo-volume-schema.json\",\n  \"title\": \"GitRepoVolume\",\n  \"description\": \"Represents a volume that is populated with the contents of a git repository\",\n  \"properties\": {\n    \"directory\": {\n      \"description\": \"Target directory name. Must not contain or start with '..'.  If '.' is supplied, the volume directory will be the git repository.  Otherwise, if specified, the volume will contain the git repository in the subdirectory with the given name.\",\n      \"type\": \"string\"\n    },\n    \"repository\": {\n      \"description\": \"Repository URL\",\n      \"type\": \"string\"\n    },\n    \"revision\": {\n      \"description\": \"Commit hash for the specified revision.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\",\n  \"\
  required\": [\n    \"repository\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-git-repo-volume-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: GitRepoVolume
---
