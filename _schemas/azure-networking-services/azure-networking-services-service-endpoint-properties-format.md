---
description: The service endpoint properties.
layout: schema
name: ServiceEndpointPropertiesFormat
properties_list:
- description: A list of locations.
  name: locations
  type: array
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The type of the endpoint service.
  name: service
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-service-endpoint-properties-format-schema.json
slug: azure-networking-services-service-endpoint-properties-format
source_filename: azure-networking-services-service-endpoint-properties-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-service-endpoint-properties-format-schema.json\",\n  \"title\": \"ServiceEndpointPropertiesFormat\",\n  \"description\": \"The service endpoint properties.\",\n  \"properties\": {\n    \"locations\": {\n      \"description\": \"A list of locations.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    },\n    \"service\": {\n      \"description\": \"The\
  \ type of the endpoint service.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-service-endpoint-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ServiceEndpointPropertiesFormat
---
