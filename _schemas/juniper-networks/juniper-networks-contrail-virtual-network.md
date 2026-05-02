---
description: Schema for a Juniper Contrail (Tungsten Fabric) virtual network object. Virtual networks are the core networking abstraction in Contrail SDN, representing isolated Layer 2/3 network segments. Each virtual network is backed by VXLAN or MPLS-over-GRE tunnels across the compute fabric, with BGP EVPN providing the control plane for MAC/IP route distribution. Virtual networks can be connected to each other through network policies, service chains, or shared route targets. Contrail automatically manages distributed routing, distributed DHCP, DNS, and metadata services within each virtual network.
layout: schema
name: Juniper Contrail Virtual Network
properties_list:
- description: Virtual network UUID assigned by Contrail upon creation.
  name: uuid
  type: string
- description: 'Fully qualified name as a hierarchical path: [domain, project, virtual-network-name]. The default domain is ''default-domain''.'
  name: fq_name
  type: array
- description: Human-readable display name for the virtual network.
  name: display_name
  type: string
- description: Parent object type. Virtual networks always belong to a project.
  name: parent_type
  type: string
- description: UUID of the parent project.
  name: parent_uuid
  type: string
- description: Core virtual network properties controlling forwarding behavior and VXLAN encapsulation.
  name: virtual_network_properties
  type: object
- description: References to IP Address Management (IPAM) objects with subnet configurations. Each reference links an IPAM object and defines the subnets allocated from it.
  name: network_ipam_refs
  type: array
- description: References to network policies attached to this virtual network. Policies control traffic flow between virtual networks.
  name: network_policy_refs
  type: array
- description: BGP route targets for the virtual network. Route targets control VPN route import/export between VRFs on gateway routers.
  name: route_target_list
  type: object
- description: Additional import-only route targets.
  name: import_route_target_list
  type: object
- description: Additional export-only route targets.
  name: export_route_target_list
  type: object
- description: Whether the virtual network is shared across all projects in the domain. Shared networks are accessible by workloads in any project.
  name: is_shared
  type: boolean
- description: Whether the virtual network provides external (internet/WAN) connectivity. External networks are connected to physical gateway routers via BGP.
  name: router_external
  type: boolean
- description: Whether to flood unknown unicast traffic within the virtual network. When false (default), Contrail uses proxy ARP/ND to avoid flooding.
  name: flood_unknown_unicast
  type: boolean
- description: Whether multiple service chains can be applied to traffic between this network and connected networks.
  name: multi_policy_service_chains_enabled
  type: boolean
provider_name: Juniper Networks
provider_slug: juniper-networks
schema_file: json-schema/juniper-networks-contrail-virtual-network-schema.json
slug: juniper-networks-contrail-virtual-network
source_filename: juniper-networks-contrail-virtual-network-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-contrail-virtual-network-schema.json\",\n  \"title\": \"Juniper Contrail Virtual Network\",\n  \"description\": \"Schema for a Juniper Contrail (Tungsten Fabric) virtual network object. Virtual networks are the core networking abstraction in Contrail SDN, representing isolated Layer 2/3 network segments. Each virtual network is backed by VXLAN or MPLS-over-GRE tunnels across the compute fabric, with BGP EVPN providing the control plane for MAC/IP route distribution. Virtual networks can be connected to each other through network policies, service chains, or shared route targets. Contrail automatically manages distributed routing, distributed DHCP, DNS, and metadata services within each virtual network.\",\n  \"type\": \"object\",\n  \"required\": [\"fq_name\"],\n  \"properties\": {\n\
  \    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Virtual network UUID assigned by Contrail upon creation.\"\n    },\n    \"fq_name\": {\n      \"type\": \"array\",\n      \"description\": \"Fully qualified name as a hierarchical path: [domain, project, virtual-network-name]. The default domain is 'default-domain'.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 3,\n      \"maxItems\": 3\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable display name for the virtual network.\"\n    },\n    \"parent_type\": {\n      \"type\": \"string\",\n      \"const\": \"project\",\n      \"description\": \"Parent object type. Virtual networks always belong to a project.\"\n    },\n    \"parent_uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"UUID of the parent project.\"\n    },\n    \"virtual_network_properties\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Core virtual network properties controlling forwarding behavior and VXLAN encapsulation.\",\n      \"properties\": {\n        \"vxlan_network_identifier\": {\n          \"type\": [\"integer\", \"null\"],\n          \"description\": \"User-configured VXLAN Network Identifier (VNI). If null, Contrail auto-assigns from the global VNI pool.\",\n          \"minimum\": 1,\n          \"maximum\": 16777215\n        },\n        \"forwarding_mode\": {\n          \"type\": \"string\",\n          \"enum\": [\"l2_l3\", \"l2\", \"l3\"],\n          \"description\": \"Forwarding mode. 'l2_l3' enables both bridging and routing (most common), 'l2' for pure bridging, 'l3' for pure routing.\",\n          \"default\": \"l2_l3\"\n        },\n        \"rpf\": {\n          \"type\": \"string\",\n          \"enum\": [\"enable\", \"disable\"],\n          \"description\": \"Reverse Path Forwarding check. When enabled, packets with source addresses not in the\
  \ routing table are dropped.\",\n          \"default\": \"enable\"\n        },\n        \"allow_transit\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether transit traffic (traffic neither sourced from nor destined to this VN) is allowed through the network.\"\n        },\n        \"mirror_destination\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this virtual network is a traffic mirror destination network.\"\n        }\n      }\n    },\n    \"network_ipam_refs\": {\n      \"type\": \"array\",\n      \"description\": \"References to IP Address Management (IPAM) objects with subnet configurations. Each reference links an IPAM object and defines the subnets allocated from it.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"to\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            },\n            \"description\": \"Fully qualified\
  \ name of the referenced IPAM object.\"\n          },\n          \"uuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\",\n            \"description\": \"IPAM object UUID.\"\n          },\n          \"attr\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"ipam_subnets\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"$ref\": \"#/$defs/IpamSubnet\"\n                },\n                \"description\": \"Subnet configurations allocated from this IPAM.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"network_policy_refs\": {\n      \"type\": \"array\",\n      \"description\": \"References to network policies attached to this virtual network. Policies control traffic flow between virtual networks.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"to\": {\n            \"type\": \"array\",\n            \"items\"\
  : {\n              \"type\": \"string\"\n            }\n          },\n          \"uuid\": {\n            \"type\": \"string\",\n            \"format\": \"uuid\"\n          },\n          \"attr\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"sequence\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"major\": {\n                    \"type\": \"integer\"\n                  },\n                  \"minor\": {\n                    \"type\": \"integer\"\n                  }\n                },\n                \"description\": \"Policy evaluation order.\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"route_target_list\": {\n      \"type\": \"object\",\n      \"description\": \"BGP route targets for the virtual network. Route targets control VPN route import/export between VRFs on gateway routers.\",\n      \"properties\": {\n        \"route_target\": {\n          \"type\"\
  : \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"pattern\": \"^target:\\\\d+:\\\\d+$\"\n          },\n          \"description\": \"List of route targets in format target:ASN:number.\"\n        }\n      }\n    },\n    \"import_route_target_list\": {\n      \"type\": \"object\",\n      \"description\": \"Additional import-only route targets.\",\n      \"properties\": {\n        \"route_target\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"export_route_target_list\": {\n      \"type\": \"object\",\n      \"description\": \"Additional export-only route targets.\",\n      \"properties\": {\n        \"route_target\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"is_shared\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the virtual network is shared\
  \ across all projects in the domain. Shared networks are accessible by workloads in any project.\",\n      \"default\": false\n    },\n    \"router_external\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the virtual network provides external (internet/WAN) connectivity. External networks are connected to physical gateway routers via BGP.\",\n      \"default\": false\n    },\n    \"flood_unknown_unicast\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to flood unknown unicast traffic within the virtual network. When false (default), Contrail uses proxy ARP/ND to avoid flooding.\",\n      \"default\": false\n    },\n    \"multi_policy_service_chains_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether multiple service chains can be applied to traffic between this network and connected networks.\"\n    }\n  },\n  \"$defs\": {\n    \"IpamSubnet\": {\n      \"type\": \"object\",\n      \"description\": \"Subnet configuration\
  \ within an IPAM reference, defining the IP address range and gateway for workloads in the virtual network.\",\n      \"properties\": {\n        \"subnet\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"ip_prefix\": {\n              \"type\": \"string\",\n              \"description\": \"IP address prefix (e.g., 10.1.1.0).\"\n            },\n            \"ip_prefix_len\": {\n              \"type\": \"integer\",\n              \"description\": \"Prefix length (e.g., 24 for /24).\",\n              \"minimum\": 0,\n              \"maximum\": 128\n            }\n          },\n          \"required\": [\"ip_prefix\", \"ip_prefix_len\"]\n        },\n        \"default_gateway\": {\n          \"type\": \"string\",\n          \"description\": \"Default gateway IP address for the subnet. Contrail distributes this gateway across all compute nodes hosting workloads in the subnet.\"\n        },\n        \"dns_server_address\": {\n          \"type\": \"string\",\n   \
  \       \"description\": \"DNS server IP address provided to workloads via DHCP.\"\n        },\n        \"enable_dhcp\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether Contrail provides distributed DHCP service for this subnet.\",\n          \"default\": true\n        },\n        \"addr_from_start\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to allocate IP addresses from the start of the subnet range.\",\n          \"default\": true\n        },\n        \"allocation_pools\": {\n          \"type\": \"array\",\n          \"description\": \"Specific IP ranges within the subnet available for dynamic allocation.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"start\": {\n                \"type\": \"string\",\n                \"description\": \"First IP in the allocation range.\"\n              },\n              \"end\": {\n                \"type\": \"string\",\n         \
  \       \"description\": \"Last IP in the allocation range.\"\n              }\n            }\n          }\n        },\n        \"subnet_uuid\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Subnet unique identifier.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-contrail-virtual-network-schema.json
tags:
- Automation
- Cloud
- Data Center
- Enterprise
- Networking
- SDN
- Security
title: Juniper Contrail Virtual Network
---
