---
description: Authorization info used to access a resource (like code repository).
layout: schema
name: Authorization
properties_list:
- description: Type of authorization.
  name: authorizationType
  type: string
- description: Authorization parameters corresponding to the authorization type.
  name: parameters
  type: object
provider_name: Azure DevOps
provider_slug: azure-dev-ops
schema_file: json-schema/azure-dev-ops-authorization-schema.json
slug: azure-dev-ops-authorization
tags:
- Azure
- CI/CD
- DevOps
- Project Management
- Version Control
title: Authorization
---
