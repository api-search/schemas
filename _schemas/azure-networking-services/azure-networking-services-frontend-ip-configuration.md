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
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: FrontendIPConfiguration
---
