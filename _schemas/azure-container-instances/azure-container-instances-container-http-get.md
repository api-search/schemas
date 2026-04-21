---
description: The container Http Get settings, for liveness or readiness probe
layout: schema
name: ContainerHttpGet
properties_list:
- description: The path to probe.
  name: path
  type: string
- description: The port number to probe.
  name: port
  type: integer
- description: The scheme.
  name: scheme
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-http-get-schema.json
slug: azure-container-instances-container-http-get
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerHttpGet
---
