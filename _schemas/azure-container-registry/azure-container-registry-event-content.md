---
description: The content of the event request message.
layout: schema
name: EventContent
properties_list:
- description: The action that encompasses the provided event.
  name: action
  type: string
- description: The agent that initiated the event. For most situations, this could be from the authorization context of the request.
  name: actor
  type: object
- description: The event ID.
  name: id
  type: string
- description: The request that generated the event.
  name: request
  type: object
- description: The registry node that generated the event. Put differently, while the actor initiates the event, the source generates it.
  name: source
  type: object
- description: The target of the event.
  name: target
  type: object
- description: The time at which the event occurred.
  name: timestamp
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-content-schema.json
slug: azure-container-registry-event-content
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EventContent
---
