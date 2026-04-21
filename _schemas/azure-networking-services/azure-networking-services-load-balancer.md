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
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: LoadBalancer
---
