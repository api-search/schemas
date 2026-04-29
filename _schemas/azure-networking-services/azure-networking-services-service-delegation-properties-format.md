---
description: Properties of a service delegation.
layout: schema
name: ServiceDelegationPropertiesFormat
properties_list:
- description: Describes the actions permitted to the service upon delegation.
  name: actions
  type: array
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The name of the service to whom the subnet should be delegated (e.g. Microsoft.Sql/servers).
  name: serviceName
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-service-delegation-properties-format-schema.json
slug: azure-networking-services-service-delegation-properties-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-service-delegation-properties-format-schema.json\",\n  \"title\": \"ServiceDelegationPropertiesFormat\",\n  \"description\": \"Properties of a service delegation.\",\n  \"properties\": {\n    \"actions\": {\n      \"description\": \"Describes the actions permitted to the service upon delegation.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    },\n\
  \    \"serviceName\": {\n      \"description\": \"The name of the service to whom the subnet should be delegated (e.g. Microsoft.Sql/servers).\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-service-delegation-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ServiceDelegationPropertiesFormat
---
