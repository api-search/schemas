---
description: The container instance properties.
layout: schema
name: ContainerProperties
properties_list:
- description: The commands to execute within the container instance in exec form.
  name: command
  type: array
- description: The environment variables to set in the container instance.
  name: environmentVariables
  type: array
- description: The name of the image used to create the container instance.
  name: image
  type: string
- description: The instance view of the container instance. Only valid in response.
  name: instanceView
  type: object
- description: The liveness probe.
  name: livenessProbe
  type: object
- description: The exposed ports on the container instance.
  name: ports
  type: array
- description: The readiness probe.
  name: readinessProbe
  type: object
- description: The resource requirements of the container instance.
  name: resources
  type: object
- description: The volume mounts available to the container instance.
  name: volumeMounts
  type: array
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-properties-schema.json
slug: azure-container-instances-container-properties
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerProperties
---
