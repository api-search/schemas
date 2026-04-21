---
description: The result of a request to list events for a webhook.
layout: schema
name: EventListResult
properties_list:
- description: The URI that can be used to request the next list of events.
  name: nextLink
  type: string
- description: The list of events. Since this list may be incomplete, the nextLink field should be used to request the next list of events.
  name: value
  type: array
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-event-list-result-schema.json
slug: azure-container-registry-event-list-result
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EventListResult
---
