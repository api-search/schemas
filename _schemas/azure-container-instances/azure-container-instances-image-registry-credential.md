---
description: Image registry credential.
layout: schema
name: ImageRegistryCredential
properties_list:
- description: The password for the private registry.
  name: password
  type: string
- description: The Docker image registry server without a protocol such as "http" and "https".
  name: server
  type: string
- description: The username for the private registry.
  name: username
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-image-registry-credential-schema.json
slug: azure-container-instances-image-registry-credential
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ImageRegistryCredential
---
