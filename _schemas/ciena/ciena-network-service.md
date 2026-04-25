---
description: Schema representing a provisioned network service on the Blue Planet SDN platform.
layout: schema
name: Ciena Blue Planet Network Service
properties_list:
- description: Unique service identifier (UUID)
  name: id
  type: string
- description: Human-readable service name
  name: name
  type: string
- description: Optional service description
  name: description
  type: string
- description: Service type designation
  name: serviceType
  type: string
- description: Current operational state of the service
  name: state
  type: string
- description: Administrative state
  name: adminState
  type: string
- description: Service bandwidth specification
  name: bandwidth
  type: string
- description: Service protection scheme
  name: protectionType
  type: string
- description: Service termination endpoints (A and Z ends)
  name: endpoints
  type: array
- description: Computed route through the network
  name: route
  type: array
- description: ''
  name: customerInfo
  type: object
- description: Service creation timestamp
  name: createdAt
  type: string
- description: Service provisioning completion timestamp
  name: provisionedAt
  type: string
- description: Last modification timestamp
  name: updatedAt
  type: string
- description: Custom key-value metadata tags
  name: tags
  type: object
provider_name: Ciena
provider_slug: ciena
schema_file: json-schema/ciena-network-service-schema.json
slug: ciena-network-service
tags:
- MEF
- NETCONF
- Network Automation
- Network Management
- Optical
- RESTCONF
- SDN
- Telecom
- TM Forum
title: Ciena Blue Planet Network Service
---
