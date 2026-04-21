---
description: Configuration used to bootstrap a Pipeline.
layout: schema
name: BootstrapConfiguration
properties_list:
- description: Repository containing the source code for the pipeline.
  name: repository
  type: object
- description: Template used to bootstrap the pipeline.
  name: template
  type: object
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-bootstrap-configuration-schema.json
slug: azure-dev-ops-bootstrap-configuration
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: BootstrapConfiguration
---
