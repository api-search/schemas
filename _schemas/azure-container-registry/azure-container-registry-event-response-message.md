---
description: The event response message received from the service URI.
layout: schema
name: EventResponseMessage
properties_list:
- description: The content of the event response message.
  name: content
  type: string
- description: The headers of the event response message.
  name: headers
  type: object
- description: The reason phrase of the event response message.
  name: reasonPhrase
  type: string
- description: The status code of the event response message.
  name: statusCode
  type: string
- description: The HTTP message version.
  name: version
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-response-message-schema.json
slug: azure-container-registry-event-response-message
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EventResponseMessage
---
