---
description: A machine catalog defines a collection of virtual or physical machines managed as a single entity for provisioning in Citrix DaaS or Virtual Apps and Desktops.
layout: schema
name: Citrix Machine Catalog
properties_list:
- description: Unique identifier for the machine catalog
  name: id
  type: string
- description: Name of the machine catalog
  name: name
  type: string
- description: Description of the machine catalog
  name: description
  type: string
- description: How machines are allocated to users
  name: allocationType
  type: string
- description: Provisioning method for machines in the catalog
  name: provisioningType
  type: string
- description: Whether machines support single or multiple concurrent sessions
  name: sessionSupport
  type: string
- description: Number of machines in the catalog
  name: machineCount
  type: integer
- description: ''
  name: zone
  type: object
provider_name: Citrix
provider_slug: citrix
schema_file: json-schema/citrix-machine-catalog-schema.json
slug: citrix-machine-catalog
tags:
- Application Delivery
- Desktop-As-A-Service
- Networking
- Virtualization
- Workspace
title: Citrix Machine Catalog
---
