---
description: Inbound NAT pool of the load balancer.
layout: schema
name: InboundNatPool
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within the set of inbound NAT pools used by the load balancer. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of load balancer inbound nat pool.
  name: properties
  type: object
- description: Type of the resource.
  name: type
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-inbound-nat-pool-schema.json
slug: azure-networking-services-inbound-nat-pool
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: InboundNatPool
---
