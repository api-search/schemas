---
description: The container instance state.
layout: schema
name: ContainerState
properties_list:
- description: The human-readable status of the container instance state.
  name: detailStatus
  type: string
- description: The container instance exit codes correspond to those from the `docker run` command.
  name: exitCode
  type: integer
- description: The date-time when the container instance state finished.
  name: finishTime
  type: string
- description: The date-time when the container instance state started.
  name: startTime
  type: string
- description: The state of the container instance.
  name: state
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-state-schema.json
slug: azure-container-instances-container-state
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerState
---
