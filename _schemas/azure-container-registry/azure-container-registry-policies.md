---
description: The policies for a container registry.
layout: schema
name: Policies
properties_list:
- description: The quarantine policy for a container registry.
  name: quarantinePolicy
  type: object
- description: The retention policy for a container registry.
  name: retentionPolicy
  type: object
- description: The content trust policy for a container registry.
  name: trustPolicy
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-policies-schema.json
slug: azure-container-registry-policies
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: Policies
---
