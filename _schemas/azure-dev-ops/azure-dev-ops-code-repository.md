---
description: Repository containing the source code for a pipeline.
layout: schema
name: CodeRepository
properties_list:
- description: Authorization info to access the code repository.
  name: authorization
  type: object
- description: Default branch used to configure Continuous Integration (CI) in the pipeline.
  name: defaultBranch
  type: string
- description: Unique immutable identifier of the code repository.
  name: id
  type: string
- description: Repository-specific properties.
  name: properties
  type: object
- description: Type of code repository.
  name: repositoryType
  type: string
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-code-repository-schema.json
slug: azure-dev-ops-code-repository
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: CodeRepository
---
