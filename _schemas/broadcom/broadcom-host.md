---
description: A Host represents a physical ESXi server that provides compute, memory, storage, and networking resources to virtual machines within a vSphere or VCF environment.
layout: schema
name: Broadcom Host
properties_list:
- description: The unique identifier of the host.
  name: id
  type: string
- description: The hostname or display name of the host.
  name: name
  type: string
- description: The fully qualified domain name of the host.
  name: fqdn
  type: string
- description: The connection state of the host.
  name: connection_state
  type: string
- description: The power state of the host.
  name: power_state
  type: string
- description: The identifier of the cluster to which this host belongs.
  name: cluster
  type: string
- description: CPU resource information for the host.
  name: cpu
  type: object
- description: Memory resource information for the host.
  name: memory
  type: object
- description: The ESXi version running on the host.
  name: version
  type: string
- description: The commissioning status of the host in VCF.
  name: status
  type: string
- description: Network addresses assigned to the host.
  name: ip_addresses
  type: array
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-host-schema.json
slug: broadcom-host
source_filename: broadcom-host-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/broadcom/blob/main/json-schema/broadcom-host-schema.json\",\n  \"title\": \"Broadcom Host\",\n  \"description\": \"A Host represents a physical ESXi server that provides compute, memory, storage, and networking resources to virtual machines within a vSphere or VCF environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the host.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname or display name of the host.\"\n    },\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified domain name of the host.\"\n    },\n    \"connection_state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONNECTED\",\n        \"DISCONNECTED\",\n        \"NOT_RESPONDING\"\n      ],\n      \"description\"\
  : \"The connection state of the host.\"\n    },\n    \"power_state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POWERED_ON\",\n        \"POWERED_OFF\",\n        \"STANDBY\"\n      ],\n      \"description\": \"The power state of the host.\"\n    },\n    \"cluster\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the cluster to which this host belongs.\"\n    },\n    \"cpu\": {\n      \"type\": \"object\",\n      \"description\": \"CPU resource information for the host.\",\n      \"properties\": {\n        \"cores\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of CPU cores.\"\n        },\n        \"frequency_MHz\": {\n          \"type\": \"integer\",\n          \"description\": \"The CPU frequency in megahertz.\"\n        },\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"The CPU model name.\"\n        }\n      }\n    },\n    \"memory\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Memory resource information for the host.\",\n      \"properties\": {\n        \"total_MiB\": {\n          \"type\": \"integer\",\n          \"description\": \"Total physical memory in mebibytes.\"\n        },\n        \"used_MiB\": {\n          \"type\": \"integer\",\n          \"description\": \"Used physical memory in mebibytes.\"\n        }\n      }\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The ESXi version running on the host.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ASSIGNED\",\n        \"UNASSIGNED_USEABLE\",\n        \"UNASSIGNED_UNUSEABLE\"\n      ],\n      \"description\": \"The commissioning status of the host in VCF.\"\n    },\n    \"ip_addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"ip_address\": {\n            \"type\": \"string\",\n            \"description\": \"The IP address.\"\
  \n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"MANAGEMENT\",\n              \"VMOTION\",\n              \"VSAN\"\n            ],\n            \"description\": \"The type of network associated with this IP.\"\n          }\n        }\n      },\n      \"description\": \"Network addresses assigned to the host.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/json-schema/broadcom-host-schema.json
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Host
---
