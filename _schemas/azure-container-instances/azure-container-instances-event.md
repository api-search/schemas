---
description: A container group or container instance event.
layout: schema
name: Event
properties_list:
- description: The count of the event.
  name: count
  type: integer
- description: The date-time of the earliest logged event.
  name: firstTimestamp
  type: string
- description: The date-time of the latest logged event.
  name: lastTimestamp
  type: string
- description: The event message.
  name: message
  type: string
- description: The event name.
  name: name
  type: string
- description: The event type.
  name: type
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-event-schema.json
slug: azure-container-instances-event
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: Event
---
