---
description: The container probe, for liveness or readiness
layout: schema
name: ContainerProbe
properties_list:
- description: The execution command to probe
  name: exec
  type: object
- description: The failure threshold.
  name: failureThreshold
  type: integer
- description: The Http Get settings to probe
  name: httpGet
  type: object
- description: The initial delay seconds.
  name: initialDelaySeconds
  type: integer
- description: The period seconds.
  name: periodSeconds
  type: integer
- description: The success threshold.
  name: successThreshold
  type: integer
- description: The timeout seconds.
  name: timeoutSeconds
  type: integer
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-probe-schema.json
slug: azure-container-instances-container-probe
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerProbe
---
