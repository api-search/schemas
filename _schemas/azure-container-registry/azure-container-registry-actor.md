---
description: The agent that initiated the event. For most situations, this could be from the authorization context of the request.
layout: schema
name: Actor
properties_list:
- description: The subject or username associated with the request context that generated the event.
  name: name
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-actor-schema.json
slug: azure-container-registry-actor
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: Actor
---
