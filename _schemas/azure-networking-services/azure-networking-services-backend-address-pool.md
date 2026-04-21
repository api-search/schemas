---
description: Pool of backend IP addresses.
layout: schema
name: BackendAddressPool
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within the set of backend address pools used by the load balancer. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of load balancer backend address pool.
  name: properties
  type: object
- description: Type of the resource.
  name: type
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-backend-address-pool-schema.json
slug: azure-networking-services-backend-address-pool
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: BackendAddressPool
---
