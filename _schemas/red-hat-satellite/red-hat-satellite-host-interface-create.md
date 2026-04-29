---
description: Parameters for creating or updating a host network interface.
layout: schema
name: HostInterfaceCreate
properties_list:
- description: Interface identifier (for updating existing interfaces).
  name: id
  type: integer
- description: MAC address.
  name: mac
  type: string
- description: IPv4 address.
  name: ip
  type: string
- description: IPv6 address.
  name: ip6
  type: string
- description: Interface type.
  name: type
  type: string
- description: DNS name.
  name: name
  type: string
- description: IPv4 subnet identifier.
  name: subnet_id
  type: integer
- description: IPv6 subnet identifier.
  name: subnet6_id
  type: integer
- description: Domain identifier.
  name: domain_id
  type: integer
- description: Device identifier (e.g., eth0).
  name: identifier
  type: string
- description: Whether DNS and DHCP are managed for this interface.
  name: managed
  type: boolean
- description: Whether this is the primary interface for FQDN.
  name: primary
  type: boolean
- description: Whether this interface is used for provisioning.
  name: provision
  type: boolean
- description: Whether this is a virtual interface (alias or VLAN).
  name: virtual
  type: boolean
- description: VLAN tag.
  name: tag
  type: string
- description: Maximum transmission unit.
  name: mtu
  type: integer
- description: Parent interface identifier.
  name: attached_to
  type: string
- description: BMC username (BMC interfaces only).
  name: username
  type: string
- description: BMC password (BMC interfaces only).
  name: password
  type: string
- description: BMC provider (BMC interfaces only).
  name: provider
  type: string
- description: Bond mode (bond interfaces only).
  name: mode
  type: string
- description: Slave or bridge member interface identifiers.
  name: attached_devices
  type: array
- description: Additional bond options (space-separated).
  name: bond_options
  type: string
provider_name: Red Hat Satellite
provider_slug: red-hat-satellite
schema_file: json-schema/red-hat-satellite-host-interface-create-schema.json
slug: red-hat-satellite-host-interface-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HostInterfaceCreate\",\n  \"type\": \"object\",\n  \"description\": \"Parameters for creating or updating a host network interface.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Interface identifier (for updating existing interfaces).\"\n    },\n    \"mac\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address.\"\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"IPv4 address.\"\n    },\n    \"ip6\": {\n      \"type\": \"string\",\n      \"description\": \"IPv6 address.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Interface type.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"DNS name.\"\n    },\n    \"subnet_id\": {\n      \"type\": \"integer\",\n      \"description\": \"IPv4 subnet identifier.\"\n    },\n    \"subnet6_id\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"IPv6 subnet identifier.\"\n    },\n    \"domain_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Domain identifier.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"Device identifier (e.g., eth0).\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether DNS and DHCP are managed for this interface.\"\n    },\n    \"primary\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary interface for FQDN.\"\n    },\n    \"provision\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this interface is used for provisioning.\"\n    },\n    \"virtual\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a virtual interface (alias or VLAN).\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"VLAN tag.\"\n    },\n    \"mtu\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"Maximum transmission unit.\"\n    },\n    \"attached_to\": {\n      \"type\": \"string\",\n      \"description\": \"Parent interface identifier.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"BMC username (BMC interfaces only).\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"BMC password (BMC interfaces only).\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"BMC provider (BMC interfaces only).\"\n    },\n    \"mode\": {\n      \"type\": \"string\",\n      \"description\": \"Bond mode (bond interfaces only).\"\n    },\n    \"attached_devices\": {\n      \"type\": \"array\",\n      \"description\": \"Slave or bridge member interface identifiers.\"\n    },\n    \"bond_options\": {\n      \"type\": \"string\",\n      \"description\": \"Additional bond options (space-separated).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-satellite/refs/heads/main/json-schema/red-hat-satellite-host-interface-create-schema.json
tags:
- Configuration Management
- Lifecycle Management
- Patch Management
- Subscription Management
- Systems Management
title: HostInterfaceCreate
---
