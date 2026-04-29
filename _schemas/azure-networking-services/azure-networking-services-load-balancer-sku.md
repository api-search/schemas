---
description: SKU of a load balancer.
layout: schema
name: LoadBalancerSku
properties_list:
- description: Name of a load balancer SKU.
  name: name
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-load-balancer-sku-schema.json
slug: azure-networking-services-load-balancer-sku
source_filename: azure-networking-services-load-balancer-sku-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-sku-schema.json\",\n  \"title\": \"LoadBalancerSku\",\n  \"description\": \"SKU of a load balancer.\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"Name of a load balancer SKU.\",\n      \"enum\": [\n        \"Basic\",\n        \"Standard\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"LoadBalancerSkuName\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-load-balancer-sku-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: LoadBalancerSku
---
