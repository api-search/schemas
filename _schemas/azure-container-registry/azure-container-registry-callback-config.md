---
description: The configuration of service URI and custom headers for the webhook.
layout: schema
name: CallbackConfig
properties_list:
- description: Custom headers that will be added to the webhook notifications.
  name: customHeaders
  type: object
- description: The service URI for the webhook to post notifications.
  name: serviceUri
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-callback-config-schema.json
slug: azure-container-registry-callback-config
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: CallbackConfig
---
