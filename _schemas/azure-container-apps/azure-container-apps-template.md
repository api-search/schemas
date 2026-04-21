---
description: Container App versioned application definition.
layout: schema
name: Template
properties_list:
- description: ''
  name: revisionSuffix
  type: string
- description: ''
  name: terminationGracePeriodSeconds
  type: integer
- description: ''
  name: initContainers
  type: array
- description: ''
  name: containers
  type: array
- description: ''
  name: scale
  type: object
- description: ''
  name: volumes
  type: array
- description: ''
  name: serviceBinds
  type: array
provider_name: Azure Container Apps
provider_slug: azure-container-apps
schema_file: json-schema/azure-container-apps-template-schema.json
slug: azure-container-apps-template
tags:
- Azure
- Containers
- Dapr
- Kubernetes
- Microservices
- Serverless
title: Template
---
