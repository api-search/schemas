---
description: Details the service to which the subnet is delegated.
layout: schema
name: Delegation
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within a subnet. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of a service delegation.
  name: properties
  type: object
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-delegation-schema.json
slug: azure-networking-services-delegation
source_filename: azure-networking-services-delegation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-delegation-schema.json\",\n  \"title\": \"Delegation\",\n  \"description\": \"Details the service to which the subnet is delegated.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the resource that is unique within a subnet. This name can be used to access the resource.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"description\": \"Properties of a service delegation.\",\n      \"properties\": {\n        \"actions\": {\n          \"description\": \"Describes the actions permitted to the service upon delegation.\",\n          \"items\": {\n            \"type\":\
  \ \"string\"\n          },\n          \"type\": \"array\"\n        },\n        \"provisioningState\": {\n          \"description\": \"The current provisioning state.\",\n          \"enum\": [\n            \"Succeeded\",\n            \"Updating\",\n            \"Deleting\",\n            \"Failed\"\n          ],\n          \"readOnly\": true,\n          \"type\": \"string\",\n          \"x-ms-enum\": {\n            \"modelAsString\": true,\n            \"name\": \"ProvisioningState\"\n          }\n        },\n        \"serviceName\": {\n          \"description\": \"The name of the service to whom the subnet should be delegated (e.g. Microsoft.Sql/servers).\",\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-delegation-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: Delegation
---
