---
description: Represents an Aruba wireless access point with monitoring data including radio information, client counts, and operational status.
layout: schema
name: AccessPoint
properties_list:
- description: Serial number of the access point.
  name: serial
  type: string
- description: Configured name of the access point.
  name: name
  type: string
- description: MAC address of the access point.
  name: macaddr
  type: string
- description: Hardware model.
  name: model
  type: string
- description: Current operational status.
  name: status
  type: string
- description: IP address of the access point.
  name: ip_address
  type: string
- description: Current firmware version.
  name: firmware_version
  type: string
- description: Configuration group assignment.
  name: group_name
  type: string
- description: Site assignment.
  name: site
  type: string
- description: Labels assigned to the access point.
  name: labels
  type: array
- description: Swarm/cluster identifier for the AP.
  name: swarm_id
  type: string
- description: Name of the Swarm/cluster.
  name: swarm_name
  type: string
- description: Cluster identifier.
  name: cluster_id
  type: string
- description: Deployment mode of the access point.
  name: ap_deployment_mode
  type: string
- description: Mesh role of the access point.
  name: mesh_role
  type: string
- description: Number of clients currently connected.
  name: client_count
  type: integer
- description: Uptime in seconds since last reboot.
  name: uptime
  type: integer
- description: Current CPU utilization percentage.
  name: cpu_utilization
  type: integer
- description: Total memory in bytes.
  name: mem_total
  type: integer
- description: Free memory in bytes.
  name: mem_free
  type: integer
- description: Radio interface information.
  name: radios
  type: array
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-access-point-schema.json
slug: aruba-central-access-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessPoint\",\n  \"type\": \"object\",\n  \"description\": \"Represents an Aruba wireless access point with monitoring data including radio information, client counts, and operational status.\",\n  \"properties\": {\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the access point.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Configured name of the access point.\"\n    },\n    \"macaddr\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address of the access point.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware model.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status.\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the access point.\"\n    },\n\
  \    \"firmware_version\": {\n      \"type\": \"string\",\n      \"description\": \"Current firmware version.\"\n    },\n    \"group_name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration group assignment.\"\n    },\n    \"site\": {\n      \"type\": \"string\",\n      \"description\": \"Site assignment.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels assigned to the access point.\"\n    },\n    \"swarm_id\": {\n      \"type\": \"string\",\n      \"description\": \"Swarm/cluster identifier for the AP.\"\n    },\n    \"swarm_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Swarm/cluster.\"\n    },\n    \"cluster_id\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster identifier.\"\n    },\n    \"ap_deployment_mode\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment mode of the access point.\"\n    },\n    \"mesh_role\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Mesh role of the access point.\"\n    },\n    \"client_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of clients currently connected.\"\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"description\": \"Uptime in seconds since last reboot.\"\n    },\n    \"cpu_utilization\": {\n      \"type\": \"integer\",\n      \"description\": \"Current CPU utilization percentage.\"\n    },\n    \"mem_total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total memory in bytes.\"\n    },\n    \"mem_free\": {\n      \"type\": \"integer\",\n      \"description\": \"Free memory in bytes.\"\n    },\n    \"radios\": {\n      \"type\": \"array\",\n      \"description\": \"Radio interface information.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-access-point-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: AccessPoint
---
