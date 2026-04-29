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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-list-result-schema.json\",\n  \"title\": \"EventListResult\",\n  \"description\": \"The result of a request to list events for a webhook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URI that can be used to request the next list of events.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The list of events. Since this list may be incomplete, the nextLink field should be used to request the next list of events.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Event\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-event-list-result-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: EventListResult
---
