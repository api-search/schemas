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
source_filename: broadcom-cluster-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/broadcom/blob/main/json-schema/broadcom-cluster-schema.json\",\n  \"title\": \"Broadcom Cluster\",\n  \"description\": \"A Cluster represents a grouping of ESXi hosts that share resources and provide high availability, distributed resource scheduling, and vSAN storage capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cluster.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the cluster.\"\n    },\n    \"ha_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether vSphere High Availability is enabled for the cluster.\"\n    },\n    \"drs_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Distributed Resource Scheduler is enabled for the cluster.\"\n    },\n\
  \    \"drs_automation_level\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"MANUAL\",\n        \"PARTIALLY_AUTOMATED\",\n        \"FULLY_AUTOMATED\"\n      ],\n      \"description\": \"The DRS automation level for the cluster.\"\n    },\n    \"vsan_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether vSAN is enabled for the cluster.\"\n    },\n    \"host_count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of hosts in the cluster.\"\n    },\n    \"hosts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The identifiers of hosts belonging to this cluster.\"\n    },\n    \"resource_pool\": {\n      \"type\": \"string\",\n      \"description\": \"The root resource pool identifier for the cluster.\"\n    },\n    \"datacenter\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the datacenter containing this cluster.\"\n    },\n    \"\
  is_stretched\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cluster is a stretched cluster spanning multiple sites.\"\n    },\n    \"primary_datastore\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the primary datastore used by the cluster.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/json-schema/broadcom-cluster-schema.json
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Cluster
---
