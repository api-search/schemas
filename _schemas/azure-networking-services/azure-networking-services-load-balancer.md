---
description: LoadBalancer resource.
layout: schema
name: LoadBalancer
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: Properties of load balancer.
  name: properties
  type: object
- description: The load balancer SKU.
  name: sku
  type: object
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-load-balancer-schema.json
slug: azure-networking-services-load-balancer
source_filename: azure-networking-services-load-balancer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-schema.json\",\n  \"title\": \"LoadBalancer\",\n  \"description\": \"LoadBalancer resource.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/LoadBalancerPropertiesFormat\",\n      \"description\": \"Properties of load balancer.\",\n      \"x-ms-client-flatten\": true\n    },\n    \"sku\": {\n      \"$ref\": \"#/definitions/LoadBalancerSku\",\n      \"description\": \"The load balancer SKU.\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: LoadBalancer
---
