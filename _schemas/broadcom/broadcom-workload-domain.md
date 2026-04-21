---
description: A Workload Domain represents a logically isolated group of clusters in VMware Cloud Foundation that provides compute, storage, and networking resources for a specific workload type.
layout: schema
name: Broadcom Workload Domain
properties_list:
- description: The unique identifier of the workload domain.
  name: id
  type: string
- description: The name of the workload domain.
  name: name
  type: string
- description: The type of workload domain. MANAGEMENT is the initial domain, VI is a Virtual Infrastructure domain.
  name: type
  type: string
- description: The current status of the workload domain.
  name: status
  type: string
- description: The clusters that belong to this workload domain.
  name: clusters
  type: array
- description: The SSO domain identifier associated with this workload domain.
  name: ssoId
  type: string
- description: The vCenter Server associated with this workload domain.
  name: vcenter
  type: object
- description: The NSX-T cluster associated with this workload domain.
  name: nsxTCluster
  type: object
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-workload-domain-schema.json
slug: broadcom-workload-domain
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Workload Domain
---
