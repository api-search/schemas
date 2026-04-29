---
description: Subnet in a virtual network resource.
layout: schema
name: Subnet
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within a resource group. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of the subnet.
  name: properties
  type: object
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-subnet-schema.json
slug: azure-networking-services-subnet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-subnet-schema.json\",\n  \"title\": \"Subnet\",\n  \"description\": \"Subnet in a virtual network resource.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the resource that is unique within a resource group. This name can be used to access the resource.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/SubnetPropertiesFormat\",\n      \"description\": \"Properties of the subnet.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-subnet-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: Subnet
---
