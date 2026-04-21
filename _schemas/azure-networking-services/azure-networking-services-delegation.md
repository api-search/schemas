---
description: Details the service to which the subnet is delegated.
layout: schema
name: Delegation
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within a subnet. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of a service delegation.
  name: properties
  type: object
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-delegation-schema.json
slug: azure-networking-services-delegation
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: Delegation
---
