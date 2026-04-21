---
description: Result of a request to list all Azure Pipelines under a given scope.
layout: schema
name: PipelineListResult
properties_list:
- description: URL to get the next set of Pipelines, if there are any.
  name: nextLink
  type: string
- description: List of pipelines.
  name: value
  type: array
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-list-result-schema.json
slug: azure-dev-ops-pipeline-list-result
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: PipelineListResult
---
