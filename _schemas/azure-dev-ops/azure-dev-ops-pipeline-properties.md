---
description: Custom properties of a Pipeline.
layout: schema
name: PipelineProperties
properties_list:
- description: Configuration used to bootstrap the Pipeline.
  name: bootstrapConfiguration
  type: object
- description: Reference to the Azure DevOps Organization containing the Pipeline.
  name: organization
  type: object
- description: Unique identifier of the Azure Pipeline within the Azure DevOps Project.
  name: pipelineId
  type: integer
- description: Reference to the Azure DevOps Project containing the Pipeline.
  name: project
  type: object
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-properties-schema.json
slug: azure-dev-ops-pipeline-properties
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: PipelineProperties
---
