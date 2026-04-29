---
description: A virtual server resource that directs client traffic to a pool of backend servers based on an IP address and port combination.
layout: schema
name: VirtualServer
properties_list:
- description: Resource type identifier.
  name: kind
  type: string
- description: Name of the virtual server resource.
  name: name
  type: string
- description: Full path including partition.
  name: fullPath
  type: string
- description: Configuration generation counter.
  name: generation
  type: integer
- description: Self-referencing URI for this resource.
  name: selfLink
  type: string
- description: Whether the virtual contributes to the operational status of the associated virtual address.
  name: addressStatus
  type: string
- description: Automatic last hop setting for return traffic routing.
  name: autoLasthop
  type: string
- description: Whether Clustered Multi-Processing (CMP) acceleration is enabled.
  name: cmpEnabled
  type: string
- description: Maximum number of concurrent connections allowed. A value of 0 means unlimited.
  name: connectionLimit
  type: integer
- description: User-defined description of the virtual server.
  name: description
  type: string
- description: Destination IP address and service port in the format /partition/address:port or /partition/address.port.
  name: destination
  type: string
- description: When true, the virtual server does not accept new connections.
  name: disabled
  type: boolean
- description: When true, the virtual server accepts and processes traffic.
  name: enabled
  type: boolean
- description: Persistence profile to use when the primary persistence method fails.
  name: fallbackPersistence
  type: string
- description: Score value used by Global Traffic Manager for load balancing decisions.
  name: gtmScore
  type: integer
- description: IP protocol for the virtual server.
  name: ipProtocol
  type: string
- description: Network mask for the destination address. Use 255.255.255.255 for host-specific virtual servers.
  name: mask
  type: string
- description: Whether connection and persistence mirroring is enabled for high availability failover.
  name: mirror
  type: string
- description: Whether NAT64 translation is enabled.
  name: nat64
  type: string
- description: Administrative partition containing this resource.
  name: partition
  type: string
- description: Persistence profiles applied to the virtual server.
  name: persist
  type: array
- description: Default pool for directing traffic. Specified as a full path (e.g., /Common/my_pool).
  name: pool
  type: string
- description: Profiles applied to the virtual server.
  name: profiles
  type: array
- description: Maximum number of connections per second. A value of disabled or 0 means no limit.
  name: rateLimit
  type: string
- description: Scope of rate limiting.
  name: rateLimitMode
  type: string
- description: iRules applied to the virtual server.
  name: rules
  type: array
- description: Source address filter. Only connections from this network are accepted.
  name: source
  type: string
- description: Source port translation behavior.
  name: sourcePort
  type: string
- description: Current SYN Cookie protection status.
  name: synCookieStatus
  type: string
- description: Whether address translation is enabled.
  name: translateAddress
  type: string
- description: Whether port translation is enabled.
  name: translatePort
  type: string
- description: Whether VLAN filtering is enabled.
  name: vlansEnabled
  type: boolean
- description: Whether the virtual server is disabled on listed VLANs.
  name: vlansDisabled
  type: boolean
- description: List of VLANs on which the virtual server is enabled or disabled.
  name: vlans
  type: array
- description: System-assigned index for the virtual server.
  name: vsIndex
  type: integer
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-virtual-server-schema.json
slug: bigip-icontrol-rest-virtual-server
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VirtualServer\",\n  \"type\": \"object\",\n  \"description\": \"A virtual server resource that directs client traffic to a pool of backend servers based on an IP address and port combination.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the virtual server resource.\"\n    },\n    \"fullPath\": {\n      \"type\": \"string\",\n      \"description\": \"Full path including partition.\"\n    },\n    \"generation\": {\n      \"type\": \"integer\",\n      \"description\": \"Configuration generation counter.\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"description\": \"Self-referencing URI for this resource.\"\n    },\n    \"addressStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the virtual\
  \ contributes to the operational status of the associated virtual address.\"\n    },\n    \"autoLasthop\": {\n      \"type\": \"string\",\n      \"description\": \"Automatic last hop setting for return traffic routing.\"\n    },\n    \"cmpEnabled\": {\n      \"type\": \"string\",\n      \"description\": \"Whether Clustered Multi-Processing (CMP) acceleration is enabled.\"\n    },\n    \"connectionLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of concurrent connections allowed. A value of 0 means unlimited.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined description of the virtual server.\"\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination IP address and service port in the format /partition/address:port or /partition/address.port.\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, the virtual server does\
  \ not accept new connections.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, the virtual server accepts and processes traffic.\"\n    },\n    \"fallbackPersistence\": {\n      \"type\": \"string\",\n      \"description\": \"Persistence profile to use when the primary persistence method fails.\"\n    },\n    \"gtmScore\": {\n      \"type\": \"integer\",\n      \"description\": \"Score value used by Global Traffic Manager for load balancing decisions.\"\n    },\n    \"ipProtocol\": {\n      \"type\": \"string\",\n      \"description\": \"IP protocol for the virtual server.\"\n    },\n    \"mask\": {\n      \"type\": \"string\",\n      \"description\": \"Network mask for the destination address. Use 255.255.255.255 for host-specific virtual servers.\"\n    },\n    \"mirror\": {\n      \"type\": \"string\",\n      \"description\": \"Whether connection and persistence mirroring is enabled for high availability failover.\"\n    },\n    \"nat64\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Whether NAT64 translation is enabled.\"\n    },\n    \"partition\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative partition containing this resource.\"\n    },\n    \"persist\": {\n      \"type\": \"array\",\n      \"description\": \"Persistence profiles applied to the virtual server.\"\n    },\n    \"pool\": {\n      \"type\": \"string\",\n      \"description\": \"Default pool for directing traffic. Specified as a full path (e.g., /Common/my_pool).\"\n    },\n    \"profiles\": {\n      \"type\": \"array\",\n      \"description\": \"Profiles applied to the virtual server.\"\n    },\n    \"rateLimit\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum number of connections per second. A value of disabled or 0 means no limit.\"\n    },\n    \"rateLimitMode\": {\n      \"type\": \"string\",\n      \"description\": \"Scope of rate limiting.\"\n    },\n    \"rules\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"iRules applied to the virtual server.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source address filter. Only connections from this network are accepted.\"\n    },\n    \"sourcePort\": {\n      \"type\": \"string\",\n      \"description\": \"Source port translation behavior.\"\n    },\n    \"synCookieStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current SYN Cookie protection status.\"\n    },\n    \"translateAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Whether address translation is enabled.\"\n    },\n    \"translatePort\": {\n      \"type\": \"string\",\n      \"description\": \"Whether port translation is enabled.\"\n    },\n    \"vlansEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether VLAN filtering is enabled.\"\n    },\n    \"vlansDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the virtual server is disabled on listed\
  \ VLANs.\"\n    },\n    \"vlans\": {\n      \"type\": \"array\",\n      \"description\": \"List of VLANs on which the virtual server is enabled or disabled.\"\n    },\n    \"vsIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"System-assigned index for the virtual server.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-virtual-server-schema.json
tags:
- API Gateway
- Application Delivery
- Automation
- Edge Computing
- Kubernetes
- Load Balancing
- Multi-Cloud
- NGINX
- Security
- WAF
title: VirtualServer
---
