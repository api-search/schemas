---
description: Properties of ServiceAssociationLink.
layout: schema
name: ServiceAssociationLinkPropertiesFormat
properties_list:
- description: If true, the resource can be deleted.
  name: allowDelete
  type: boolean
- description: Link to the external resource.
  name: link
  type: string
- description: Resource type of the linked resource.
  name: linkedResourceType
  type: string
- description: A list of locations.
  name: locations
  type: array
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-service-association-link-properties-format-schema.json
slug: azure-networking-services-service-association-link-properties-format
source_filename: azure-networking-services-service-association-link-properties-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-service-association-link-properties-format-schema.json\",\n  \"title\": \"ServiceAssociationLinkPropertiesFormat\",\n  \"description\": \"Properties of ServiceAssociationLink.\",\n  \"properties\": {\n    \"allowDelete\": {\n      \"description\": \"If true, the resource can be deleted.\",\n      \"type\": \"boolean\"\n    },\n    \"link\": {\n      \"description\": \"Link to the external resource.\",\n      \"type\": \"string\"\n    },\n    \"linkedResourceType\": {\n      \"description\": \"Resource type of the linked resource.\",\n      \"type\": \"string\"\n    },\n    \"locations\": {\n      \"description\": \"A list of locations.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"provisioningState\": {\n   \
  \   \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-service-association-link-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ServiceAssociationLinkPropertiesFormat
---
