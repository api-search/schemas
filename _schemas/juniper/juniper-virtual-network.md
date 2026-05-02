---
description: Schema representing a virtual network across Juniper platforms including Contrail, Apstra, and Mist. Covers VXLAN overlays, VLANs, VRFs, and software-defined network segments.
layout: schema
name: Juniper Virtual Network
properties_list:
- description: Unique identifier for the virtual network
  name: id
  type: string
- description: Virtual network name
  name: name
  type: string
- description: Human-readable description
  name: description
  type: string
- description: Virtual network encapsulation type
  name: vn_type
  type: string
- description: VLAN identifier
  name: vlan_id
  type: integer
- description: VXLAN Network Identifier
  name: vni
  type: integer
- description: IP subnets associated with the virtual network
  name: subnets
  type: array
- description: Associated routing zone (VRF)
  name: routing_zone
  type: object
- description: Layer 2/3 forwarding mode
  name: forwarding_mode
  type: string
- description: BGP route targets for the virtual network
  name: route_targets
  type: object
- description: Devices where this virtual network is provisioned
  name: bound_devices
  type: array
- description: References to applied network policies
  name: network_policy_refs
  type: array
- description: Tenant or project identifier
  name: tenant_id
  type: string
- description: Organization identifier
  name: org_id
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Juniper Networks
provider_slug: juniper
schema_file: json-schema/juniper-virtual-network.json
slug: juniper-virtual-network
source_filename: juniper-virtual-network.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/juniper/json-schema/juniper-virtual-network.json\",\n  \"title\": \"Juniper Virtual Network\",\n  \"description\": \"Schema representing a virtual network across Juniper platforms including Contrail, Apstra, and Mist. Covers VXLAN overlays, VLANs, VRFs, and software-defined network segments.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the virtual network\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual network name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description\"\n    },\n    \"vn_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"vxlan\",\n        \"vlan\",\n        \"evpn\",\n        \"l3vpn\"\n      ],\n      \"description\": \"Virtual network\
  \ encapsulation type\"\n    },\n    \"vlan_id\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 4094,\n      \"description\": \"VLAN identifier\"\n    },\n    \"vni\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 16777215,\n      \"description\": \"VXLAN Network Identifier\"\n    },\n    \"subnets\": {\n      \"type\": \"array\",\n      \"description\": \"IP subnets associated with the virtual network\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"prefix\": {\n            \"type\": \"string\",\n            \"description\": \"IP prefix in CIDR notation (e.g., 10.0.1.0/24)\"\n          },\n          \"gateway\": {\n            \"type\": \"string\",\n            \"format\": \"ipv4\",\n            \"description\": \"Default gateway IP\"\n          },\n          \"dhcp_enabled\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether DHCP is enabled for this subnet\"\
  \n          },\n          \"dns_servers\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\",\n              \"format\": \"ipv4\"\n            }\n          },\n          \"address_family\": {\n            \"type\": \"string\",\n            \"enum\": [\"ipv4\", \"ipv6\"]\n          }\n        },\n        \"required\": [\"prefix\"]\n      }\n    },\n    \"routing_zone\": {\n      \"type\": \"object\",\n      \"description\": \"Associated routing zone (VRF)\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"vrf_name\": {\n          \"type\": \"string\",\n          \"description\": \"VRF name on network devices\"\n        }\n      }\n    },\n    \"forwarding_mode\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"l2\",\n        \"l3\",\n        \"l2_l3\"\n      ],\n      \"description\": \"Layer 2/3 forwarding mode\"\
  \n    },\n    \"route_targets\": {\n      \"type\": \"object\",\n      \"description\": \"BGP route targets for the virtual network\",\n      \"properties\": {\n        \"import\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"export\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"bound_devices\": {\n      \"type\": \"array\",\n      \"description\": \"Devices where this virtual network is provisioned\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"device_id\": {\n            \"type\": \"string\"\n          },\n          \"device_name\": {\n            \"type\": \"string\"\n          },\n          \"interfaces\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n\
  \    \"network_policy_refs\": {\n      \"type\": \"array\",\n      \"description\": \"References to applied network policies\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant or project identifier\"\n    },\n    \"org_id\": {\n      \"type\": \"string\",\n      \"description\": \"Organization identifier\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"vn_type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/json-schema/juniper-virtual-network.json
tags:
- AI
- Automation
- Cloud
- Enterprise
- Networking
- SDN
- Security
title: Juniper Virtual Network
---
