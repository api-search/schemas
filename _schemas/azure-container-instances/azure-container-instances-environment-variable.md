---
description: The environment variable to set within the container instance.
layout: schema
name: EnvironmentVariable
properties_list:
- description: The name of the environment variable.
  name: name
  type: string
- description: The value of the secure environment variable.
  name: secureValue
  type: string
- description: The value of the environment variable.
  name: value
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-environment-variable-schema.json
slug: azure-container-instances-environment-variable
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: EnvironmentVariable
---
