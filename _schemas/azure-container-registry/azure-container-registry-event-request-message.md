---
description: The event request message sent to the service URI.
layout: schema
name: EventRequestMessage
properties_list:
- description: The content of the event request message.
  name: content
  type: object
- description: The headers of the event request message.
  name: headers
  type: object
- description: The HTTP method used to send the event request message.
  name: method
  type: string
- description: The URI used to send the event request message.
  name: requestUri
  type: string
- description: The HTTP message version.
  name: version
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-request-message-schema.json
slug: azure-container-registry-event-request-message
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EventRequestMessage
---
