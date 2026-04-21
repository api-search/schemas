---
description: The event for a webhook.
layout: schema
name: Event
properties_list:
- description: The event request message sent to the service URI.
  name: eventRequestMessage
  type: object
- description: The event response message received from the service URI.
  name: eventResponseMessage
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-schema.json
slug: azure-container-registry-event
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: Event
---
