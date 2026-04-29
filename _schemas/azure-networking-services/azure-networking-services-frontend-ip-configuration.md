---
description: Frontend IP address of the load balancer.
layout: schema
name: FrontendIPConfiguration
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within the set of frontend IP configurations used by the load balancer. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of the load balancer probe.
  name: properties
  type: object
- description: Type of the resource.
  name: type
  type: string
- description: A list of availability zones denoting the IP allocated for the resource needs to come from.
  name: zones
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-frontend-ip-configuration-schema.json
slug: azure-networking-services-frontend-ip-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-frontend-ip-configuration-schema.json\",\n  \"title\": \"FrontendIPConfiguration\",\n  \"description\": \"Frontend IP address of the load balancer.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the resource that is unique within the set of frontend IP configurations used by the load balancer. This name can be used to access the resource.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/FrontendIPConfigurationPropertiesFormat\",\n      \"description\": \"Properties of the load balancer probe.\",\n      \"x-ms-client-flatten\": true\n    },\n\
  \    \"type\": {\n      \"description\": \"Type of the resource.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"zones\": {\n      \"description\": \"A list of availability zones denoting the IP allocated for the resource needs to come from.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-frontend-ip-configuration-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: FrontendIPConfiguration
---
