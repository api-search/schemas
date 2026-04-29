---
description: ResourceNavigationLink resource.
layout: schema
name: ResourceNavigationLink
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: Resource navigation link identifier.
  name: id
  type: string
- description: Name of the resource that is unique within a resource group. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of ResourceNavigationLink.
  name: properties
  type: object
- description: Resource type.
  name: type
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-resource-navigation-link-schema.json
slug: azure-networking-services-resource-navigation-link
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-resource-navigation-link-schema.json\",\n  \"title\": \"ResourceNavigationLink\",\n  \"description\": \"ResourceNavigationLink resource.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"Resource navigation link identifier.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name of the resource that is unique within a resource group. This name can be used to access the resource.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"description\": \"Properties of ResourceNavigationLink.\",\n      \"properties\"\
  : {\n        \"link\": {\n          \"description\": \"Link to the external resource.\",\n          \"type\": \"string\"\n        },\n        \"linkedResourceType\": {\n          \"description\": \"Resource type of the linked resource.\",\n          \"type\": \"string\"\n        },\n        \"provisioningState\": {\n          \"description\": \"The current provisioning state.\",\n          \"enum\": [\n            \"Succeeded\",\n            \"Updating\",\n            \"Deleting\",\n            \"Failed\"\n          ],\n          \"readOnly\": true,\n          \"type\": \"string\",\n          \"x-ms-enum\": {\n            \"modelAsString\": true,\n            \"name\": \"ProvisioningState\"\n          }\n        }\n      }\n    },\n    \"type\": {\n      \"description\": \"Resource type.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-resource-navigation-link-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ResourceNavigationLink
---
