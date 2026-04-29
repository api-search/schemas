---
description: VlanAttachmentRequest schema from SP Interconnect Manage APIs
layout: schema
name: VlanAttachmentRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: stackType
  type: string
- description: ''
  name: bandwidth
  type: string
- description: ''
  name: bgpPeerAsn
  type: integer
- description: ''
  name: bgpPeerBfdSessionInitMode
  type: string
- description: ''
  name: bgpPeerBfdMinTransmitInterval
  type: integer
- description: ''
  name: bgpPeerBfdMinReceiveInterval
  type: integer
- description: ''
  name: bgpPeerBfdMultiplier
  type: integer
- description: ''
  name: dedicatedConnectionDetails
  type: array
- description: Custom IP address configuration for VLAN attachment BGP peering. Both Cloud Router and Customer Router IP addresses must be provided together with matching prefix lengths (/29 or /30). IP addresses mu
  name: primaryAttachmentCustomIpAddress
  type: object
- description: Custom IP address configuration for VLAN attachment BGP peering. Both Cloud Router and Customer Router IP addresses must be provided together with matching prefix lengths (/29 or /30). IP addresses mu
  name: redundantAttachmentCustomIpAddress
  type: object
- description: ''
  name: bgpPeerMd5AuthEnabled
  type: boolean
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-interconnect-api-vlan-attachment-request-schema.json
slug: sase-multitenant-interconnect-api-vlan-attachment-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VlanAttachmentRequest\",\n  \"description\": \"VlanAttachmentRequest schema from SP Interconnect Manage APIs\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-vlan-attachment-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"pattern\": \"^([-0-9a-z]){1,13}$\"\n    },\n    \"stackType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IPV4_ONLY\",\n        \"IPV4_IPV6\"\n      ]\n    },\n    \"bandwidth\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"BPS_50M\",\n        \"BPS_100M\",\n        \"BPS_200M\",\n        \"BPS_300M\",\n        \"BPS_400M\",\n        \"BPS_500M\",\n        \"BPS_1G\",\n        \"BPS_2G\",\n        \"BPS_5G\",\n        \"BPS_10G\"\n      ]\n    },\n    \"bgpPeerAsn\": {\n\
  \      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"minimum\": 1\n    },\n    \"bgpPeerBfdSessionInitMode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"PASSIVE\",\n        \"DISABLED\"\n      ]\n    },\n    \"bgpPeerBfdMinTransmitInterval\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"maximum\": 30000,\n      \"minimum\": 1000\n    },\n    \"bgpPeerBfdMinReceiveInterval\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"maximum\": 30000,\n      \"minimum\": 1000\n    },\n    \"bgpPeerBfdMultiplier\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"maximum\": 16,\n      \"minimum\": 5\n    },\n    \"dedicatedConnectionDetails\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"edgeAvailability\": {\n            \"type\": \"string\"\n          },\n          \"bandwidth\": {\n            \"\
  type\": \"string\",\n            \"enum\": [\n              \"BPS_50M\",\n              \"BPS_100M\",\n              \"BPS_200M\",\n              \"BPS_300M\",\n              \"BPS_400M\",\n              \"BPS_500M\",\n              \"BPS_1G\",\n              \"BPS_2G\",\n              \"BPS_5G\",\n              \"BPS_10G\"\n            ]\n          }\n        },\n        \"required\": [\n          \"edgeAvailability\"\n        ]\n      }\n    },\n    \"primaryAttachmentCustomIpAddress\": {\n      \"type\": \"object\",\n      \"description\": \"Custom IP address configuration for VLAN attachment BGP peering. Both Cloud Router and Customer Router IP addresses must be provided together with matching prefix lengths (/29 or /30). IP addresses must not be in reserved ranges (RFC1918 private IPs, loopback, etc.) and must not be network or broadcast addresses.\",\n      \"properties\": {\n        \"candidateCloudRouterIpAddress\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Cloud Router IP address in CIDR notation (e.g., 169.254.1.1/29). Must have prefix length /29 or /30 and match the prefix length of candidateCustomerRouterIpAddress.\",\n          \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n        },\n        \"candidateCustomerRouterIpAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Customer Router IP address in CIDR notation (e.g., 169.254.1.2/29). Must have prefix length /29 or /30 and match the prefix length of candidateCloudRouterIpAddress.\",\n          \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n        }\n      }\n    },\n    \"redundantAttachmentCustomIpAddress\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Custom IP address configuration for VLAN attachment BGP peering. Both Cloud Router and Customer Router IP addresses must be provided together with matching prefix lengths (/29 or /30). IP addresses must not be in reserved ranges (RFC1918 private IPs, loopback, etc.) and must not be network or broadcast addresses.\",\n      \"properties\": {\n        \"candidateCloudRouterIpAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud Router IP address in CIDR notation (e.g., 169.254.1.1/29). Must have prefix length /29 or /30 and match the prefix length of candidateCustomerRouterIpAddress.\",\n          \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n        },\n        \"candidateCustomerRouterIpAddress\": {\n          \"type\": \"string\",\n          \"description\": \"Customer Router IP address in CIDR notation\
  \ (e.g., 169.254.1.2/29). Must have prefix length /29 or /30 and match the prefix length of candidateCloudRouterIpAddress.\",\n          \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n        }\n      }\n    },\n    \"bgpPeerMd5AuthEnabled\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"bgpPeerAsn\",\n    \"bgpPeerBfdSessionInitMode\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-vlan-attachment-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: VlanAttachmentRequest
---
