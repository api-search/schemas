---
description: Properties of ResourceNavigationLink.
layout: schema
name: ResourceNavigationLinkFormat
properties_list:
- description: Link to the external resource.
  name: link
  type: string
- description: Resource type of the linked resource.
  name: linkedResourceType
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-resource-navigation-link-format-schema.json
slug: azure-networking-services-resource-navigation-link-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-resource-navigation-link-format-schema.json\",\n  \"title\": \"ResourceNavigationLinkFormat\",\n  \"description\": \"Properties of ResourceNavigationLink.\",\n  \"properties\": {\n    \"link\": {\n      \"description\": \"Link to the external resource.\",\n      \"type\": \"string\"\n    },\n    \"linkedResourceType\": {\n      \"description\": \"Resource type of the linked resource.\",\n      \"type\": \"string\"\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\
  \n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-resource-navigation-link-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ResourceNavigationLinkFormat
---
