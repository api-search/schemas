---
description: InterconnectRequest schema from SP Interconnect Manage APIs
layout: schema
name: InterconnectRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: region
  type: string
- description: ''
  name: partnerName
  type: string
- description: ''
  name: partnerEmail
  type: string
- description: ''
  name: usage
  type: string
- description: ''
  name: tsgId
  type: string
- description: ''
  name: cloudProvider
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: ipPool
  type: object
- description: ''
  name: physicalConnection
  type: object
- description: ''
  name: vlanAttachment
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-interconnect-api-interconnect-request-schema.json
slug: sase-multitenant-interconnect-api-interconnect-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InterconnectRequest\",\n  \"description\": \"InterconnectRequest schema from SP Interconnect Manage APIs\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-interconnect-request-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"pattern\": \"^([-0-9a-z]){1,13}$\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"pattern\": \"\\\\\\\\S+\"\n    },\n    \"partnerName\": {\n      \"type\": \"string\",\n      \"pattern\": \"^([a-zA-Z0-9\\\\s\\\\-]){1,30}$\"\n    },\n    \"partnerEmail\": {\n      \"type\": \"string\",\n      \"pattern\": \"\\\\\\\\S\"\n    },\n    \"usage\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SHARED\",\n        \"PER_TENANT\"\n      ]\n    },\n    \"tsgId\": {\n      \"type\": \"string\"\
  ,\n      \"pattern\": \"^[0-9-]+$\"\n    },\n    \"cloudProvider\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"GCP\",\n        \"AWS\"\n      ]\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DEDICATED\",\n        \"PARTNER\"\n      ]\n    },\n    \"ipPool\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"ipProvider\"\n      ],\n      \"properties\": {\n        \"ipBlocks\": {\n          \"type\": \"array\",\n          \"uniqueItems\": true,\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\n              \"cidr\"\n            ],\n            \"properties\": {\n              \"edgeLocation\": {\n                \"type\": \"string\"\n              },\n              \"cidr\": {\n                \"type\": \"array\",\n                \"minItems\": 1,\n                \"uniqueItems\": true,\n                \"items\": {\n                  \"type\": \"string\"\n                }\n  \
  \            },\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"PRIMARY\",\n                  \"SECONDARY\"\n                ]\n              }\n            }\n          }\n        },\n        \"ipProvider\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"SP\",\n            \"PANW\"\n          ]\n        }\n      }\n    },\n    \"physicalConnection\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"physicalConnectionName\",\n        \"linkType\",\n        \"coloFacilities\",\n        \"partnerName\",\n        \"partnerEmail\"\n      ],\n      \"properties\": {\n        \"physicalConnectionName\": {\n          \"type\": \"string\",\n          \"pattern\": \"\\\\\\\\S\"\n        },\n        \"linkType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"LINK_TYPE_ETHERNET_10G_LR\",\n            \"LINK_TYPE_ETHERNET_100G_LR\"\n          ]\n        },\n    \
  \    \"requestedLinkCount\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\"\n        },\n        \"coloFacilities\": {\n          \"type\": \"array\",\n          \"minItems\": 1,\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"macSecEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"partnerName\": {\n          \"type\": \"string\",\n          \"pattern\": \"\\\\\\\\S\"\n        },\n        \"partnerEmail\": {\n          \"type\": \"string\",\n          \"pattern\": \"\\\\\\\\S\"\n        }\n      }\n    },\n    \"vlanAttachment\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"name\",\n        \"bgpPeerAsn\",\n        \"bgpPeerBfdSessionInitMode\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"pattern\": \"^([-0-9a-z]){1,13}$\"\n        },\n        \"stackType\": {\n          \"type\": \"string\",\n          \"enum\": [\n       \
  \     \"IPV4_ONLY\",\n            \"IPV4_IPV6\"\n          ]\n        },\n        \"bandwidth\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"BPS_50M\",\n            \"BPS_100M\",\n            \"BPS_200M\",\n            \"BPS_300M\",\n            \"BPS_400M\",\n            \"BPS_500M\",\n            \"BPS_1G\",\n            \"BPS_2G\",\n            \"BPS_5G\",\n            \"BPS_10G\"\n          ]\n        },\n        \"bgpPeerAsn\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"minimum\": 1\n        },\n        \"bgpPeerBfdSessionInitMode\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ACTIVE\",\n            \"PASSIVE\",\n            \"DISABLED\"\n          ]\n        },\n        \"bgpPeerBfdMinTransmitInterval\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"maximum\": 30000,\n          \"minimum\": 1000\n        },\n        \"bgpPeerBfdMinReceiveInterval\"\
  : {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"maximum\": 30000,\n          \"minimum\": 1000\n        },\n        \"bgpPeerBfdMultiplier\": {\n          \"type\": \"integer\",\n          \"format\": \"int64\",\n          \"maximum\": 16,\n          \"minimum\": 5\n        },\n        \"dedicatedConnectionDetails\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"edgeAvailability\": {\n                \"type\": \"string\"\n              },\n              \"bandwidth\": {\n                \"type\": \"string\",\n                \"enum\": [\n                  \"BPS_50M\",\n                  \"BPS_100M\",\n                  \"BPS_200M\",\n                  \"BPS_300M\",\n                  \"BPS_400M\",\n                  \"BPS_500M\",\n                  \"BPS_1G\",\n                  \"BPS_2G\",\n                  \"BPS_5G\",\n                  \"BPS_10G\"\n  \
  \              ]\n              }\n            },\n            \"required\": [\n              \"edgeAvailability\"\n            ]\n          }\n        },\n        \"primaryAttachmentCustomIpAddress\": {\n          \"type\": \"object\",\n          \"description\": \"Custom IP address configuration for VLAN attachment BGP peering. Both Cloud Router and Customer Router IP addresses must be provided together with matching prefix lengths (/29 or /30). IP addresses must not be in reserved ranges (RFC1918 private IPs, loopback, etc.) and must not be network or broadcast addresses.\",\n          \"properties\": {\n            \"candidateCloudRouterIpAddress\": {\n              \"type\": \"string\",\n              \"description\": \"Cloud Router IP address in CIDR notation (e.g., 169.254.1.1/29). Must have prefix length /29 or /30 and match the prefix length of candidateCustomerRouterIpAddress.\",\n              \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\
  \\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n            },\n            \"candidateCustomerRouterIpAddress\": {\n              \"type\": \"string\",\n              \"description\": \"Customer Router IP address in CIDR notation (e.g., 169.254.1.2/29). Must have prefix length /29 or /30 and match the prefix length of candidateCloudRouterIpAddress.\",\n              \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n            }\n          }\n        },\n        \"redundantAttachmentCustomIpAddress\": {\n          \"type\": \"object\",\n          \"description\": \"Custom IP address configuration for VLAN attachment BGP peering. Both Cloud Router and Customer Router IP addresses must be provided together with matching prefix lengths (/29 or /30). IP addresses must not be in reserved ranges\
  \ (RFC1918 private IPs, loopback, etc.) and must not be network or broadcast addresses.\",\n          \"properties\": {\n            \"candidateCloudRouterIpAddress\": {\n              \"type\": \"string\",\n              \"description\": \"Cloud Router IP address in CIDR notation (e.g., 169.254.1.1/29). Must have prefix length /29 or /30 and match the prefix length of candidateCustomerRouterIpAddress.\",\n              \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n            },\n            \"candidateCustomerRouterIpAddress\": {\n              \"type\": \"string\",\n              \"description\": \"Customer Router IP address in CIDR notation (e.g., 169.254.1.2/29). Must have prefix length /29 or /30 and match the prefix length of candidateCloudRouterIpAddress.\",\n              \"pattern\": \"^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\
  \\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\\\\.(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?))/(29|30)$\"\n            }\n          }\n        },\n        \"bgpPeerMd5AuthEnabled\": {\n          \"type\": \"boolean\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"region\",\n    \"partnerName\",\n    \"partnerEmail\",\n    \"usage\",\n    \"cloudProvider\",\n    \"type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-interconnect-request-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: InterconnectRequest
---
