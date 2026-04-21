---
description: Definition of a pipeline template.
layout: schema
name: PipelineTemplateDefinition
properties_list:
- description: Description of the pipeline enabled by the template.
  name: description
  type: string
- description: Unique identifier of the pipeline template.
  name: id
  type: string
- description: List of input parameters required by the template to create a pipeline.
  name: inputs
  type: array
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-pipeline-template-definition-schema.json
slug: azure-dev-ops-pipeline-template-definition
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: PipelineTemplateDefinition
---
