---
description: A CloudStack availability zone grouping compute, network, and storage resources.
layout: schema
name: Zone
properties_list:
- description: UUID of the zone.
  name: id
  type: string
- description: Name of the zone.
  name: name
  type: string
- description: Network type of the zone (Basic or Advanced).
  name: networktype
  type: string
- description: Allocation state of the zone (Enabled or Disabled).
  name: allocationstate
  type: string
- description: Whether security groups are enabled in the zone.
  name: securitygroupsenabled
  type: boolean
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
schema_file: json-schema/cloudstack-api-zone-schema.json
slug: cloudstack-api-zone
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: Zone
---
