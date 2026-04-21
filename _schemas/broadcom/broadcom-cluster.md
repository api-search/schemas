---
description: A Cluster represents a grouping of ESXi hosts that share resources and provide high availability, distributed resource scheduling, and vSAN storage capabilities.
layout: schema
name: Broadcom Cluster
properties_list:
- description: The unique identifier of the cluster.
  name: id
  type: string
- description: The display name of the cluster.
  name: name
  type: string
- description: Whether vSphere High Availability is enabled for the cluster.
  name: ha_enabled
  type: boolean
- description: Whether Distributed Resource Scheduler is enabled for the cluster.
  name: drs_enabled
  type: boolean
- description: The DRS automation level for the cluster.
  name: drs_automation_level
  type: string
- description: Whether vSAN is enabled for the cluster.
  name: vsan_enabled
  type: boolean
- description: The number of hosts in the cluster.
  name: host_count
  type: integer
- description: The identifiers of hosts belonging to this cluster.
  name: hosts
  type: array
- description: The root resource pool identifier for the cluster.
  name: resource_pool
  type: string
- description: The identifier of the datacenter containing this cluster.
  name: datacenter
  type: string
- description: Whether the cluster is a stretched cluster spanning multiple sites.
  name: is_stretched
  type: boolean
- description: The identifier of the primary datastore used by the cluster.
  name: primary_datastore
  type: string
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-cluster-schema.json
slug: broadcom-cluster
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Cluster
---
