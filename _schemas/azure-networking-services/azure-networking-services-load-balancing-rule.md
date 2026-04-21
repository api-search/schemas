---
description: A load balancing rule for a load balancer.
layout: schema
name: LoadBalancingRule
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within the set of load balancing rules used by the load balancer. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of load balancer load balancing rule.
  name: properties
  type: object
- description: Type of the resource.
  name: type
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-load-balancing-rule-schema.json
slug: azure-networking-services-load-balancing-rule
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: LoadBalancingRule
---
