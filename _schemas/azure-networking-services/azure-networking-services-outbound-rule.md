---
description: Outbound rule of the load balancer.
layout: schema
name: OutboundRule
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within the set of outbound rules used by the load balancer. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of load balancer outbound rule.
  name: properties
  type: object
- description: Type of the resource.
  name: type
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-outbound-rule-schema.json
slug: azure-networking-services-outbound-rule
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: OutboundRule
---
