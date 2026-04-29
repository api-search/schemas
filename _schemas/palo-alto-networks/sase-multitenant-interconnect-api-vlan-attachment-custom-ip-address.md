---
description: Custom IP address configuration for VLAN attachment BGP peering. Both Cloud Router and Customer Router IP addresses must be provided together with matching prefix lengths (/29 or /30). IP addresses must not be in reserved ranges (RFC1918 private IPs, loopback, etc.) and must not be network or broadcast addresses.
layout: schema
name: VlanAttachmentCustomIpAddress
properties_list:
- description: Cloud Router IP address in CIDR notation (e.g., 169.254.1.1/29). Must have prefix length /29 or /30 and match the prefix length of candidateCustomerRouterIpAddress.
  name: candidateCloudRouterIpAddress
  type: string
- description: Customer Router IP address in CIDR notation (e.g., 169.254.1.2/29). Must have prefix length /29 or /30 and match the prefix length of candidateCloudRouterIpAddress.
  name: candidateCustomerRouterIpAddress
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-interconnect-api-vlan-attachment-custom-ip-address-schema.json
slug: sase-multitenant-interconnect-api-vlan-attachment-custom-ip-address
source_filename: sase-multitenant-interconnect-api-vlan-attachment-custom-ip-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VlanAttachmentCustomIpAddress\",\n  \"description\": \"Custom IP address configuration for VLAN attachment BGP peering. Both Cloud Router and Customer Router IP addresses must be provided together with matching prefix lengths (/29 or /30). IP addresses must not be in reserved ranges (RFC1918 private IPs, loopback, etc.) and must not be network or broadcast addresses.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-vlan-attachment-custom-ip-address-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"candidateCloudRouterIpAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud Router IP address in CIDR notation (e.g., 169.254.1.1/29). Must have prefix length /29 or /30 and match the prefix length of candidateCustomerRouterIpAddress.\",\n      \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\
  \\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n    },\n    \"candidateCustomerRouterIpAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Customer Router IP address in CIDR notation (e.g., 169.254.1.2/29). Must have prefix length /29 or /30 and match the prefix length of candidateCloudRouterIpAddress.\",\n      \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-vlan-attachment-custom-ip-address-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: VlanAttachmentCustomIpAddress
---
