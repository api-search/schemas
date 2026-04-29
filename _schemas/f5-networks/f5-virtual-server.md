---
description: Schema for an F5 BIG-IP LTM virtual server resource that directs client traffic to pools of backend servers based on IP address, port, and protocol configuration. Virtual servers are the core traffic management objects in the BIG-IP Local Traffic Manager.
layout: schema
name: F5 BIG-IP Virtual Server
properties_list:
- description: Resource type identifier for a virtual server.
  name: kind
  type: string
- description: Unique name of the virtual server resource within its partition.
  name: name
  type: string
- description: Full administrative path including partition (e.g., /Common/my_virtual).
  name: fullPath
  type: string
- description: Configuration generation counter incremented on each change.
  name: generation
  type: integer
- description: Self-referencing URI for this virtual server resource.
  name: selfLink
  type: string
- description: Whether the virtual contributes to the operational status of the associated virtual address.
  name: addressStatus
  type: string
- description: Automatic last hop setting controlling return traffic routing when the BIG-IP is not the default gateway.
  name: autoLasthop
  type: string
- description: Whether Clustered Multi-Processing (CMP) acceleration is enabled for this virtual server.
  name: cmpEnabled
  type: string
- description: Maximum number of concurrent connections allowed for this virtual server. A value of 0 means unlimited connections.
  name: connectionLimit
  type: integer
- description: User-defined description of the virtual server and its purpose.
  name: description
  type: string
- description: Destination IP address and service port the virtual server listens on, specified in /partition/address:port or /partition/address.port format.
  name: destination
  type: string
- description: When true, the virtual server does not accept new connections. Existing connections are maintained.
  name: disabled
  type: boolean
- description: When true, the virtual server accepts and processes client traffic.
  name: enabled
  type: boolean
- description: Persistence profile to use as a fallback when the primary persistence method fails to establish a session.
  name: fallbackPersistence
  type: string
- description: Score value used by the Global Traffic Manager for load balancing decisions across data centers.
  name: gtmScore
  type: integer
- description: Network protocol the virtual server handles.
  name: ipProtocol
  type: string
- description: Network mask for the destination address. Use 255.255.255.255 for a host-specific virtual server or a subnet mask for a network virtual server.
  name: mask
  type: string
- description: Whether connection and persistence state mirroring is enabled for high-availability failover scenarios.
  name: mirror
  type: string
- description: Whether NAT64 IPv6-to-IPv4 address translation is enabled.
  name: nat64
  type: string
- description: Administrative partition containing this virtual server resource.
  name: partition
  type: string
- description: Persistence profiles applied to the virtual server for maintaining session affinity.
  name: persist
  type: array
- description: Default pool that receives traffic from this virtual server, specified as a full partition-qualified path.
  name: pool
  type: string
- description: Traffic processing profiles applied to this virtual server (e.g., HTTP, TCP, SSL profiles).
  name: profiles
  type: array
- description: Maximum number of new connections per second. A value of 'disabled' or '0' means no rate limiting.
  name: rateLimit
  type: string
- description: Scope at which rate limiting is applied.
  name: rateLimitMode
  type: string
- description: Destination address mask bits used for rate limit tracking.
  name: rateLimitDstMask
  type: integer
- description: Source address mask bits used for rate limit tracking.
  name: rateLimitSrcMask
  type: integer
- description: iRules applied to this virtual server for custom traffic processing logic.
  name: rules
  type: array
- description: Source address filter. Only connections from this network are accepted by the virtual server.
  name: source
  type: string
- description: Source port translation behavior controlling how client source ports are handled.
  name: sourcePort
  type: string
- description: Current SYN Cookie DDoS protection status.
  name: synCookieStatus
  type: string
- description: Whether destination address translation is enabled. When enabled, the BIG-IP translates the destination address to the pool member address.
  name: translateAddress
  type: string
- description: Whether destination port translation is enabled. When enabled, the BIG-IP translates the destination port to the pool member port.
  name: translatePort
  type: string
- description: When true, the virtual server is enabled only on VLANs listed in the vlans property.
  name: vlansEnabled
  type: boolean
- description: When true, the virtual server is disabled on VLANs listed in the vlans property.
  name: vlansDisabled
  type: boolean
- description: List of VLANs on which the virtual server is enabled or disabled, depending on vlansEnabled/vlansDisabled setting.
  name: vlans
  type: array
- description: System-assigned index for the virtual server.
  name: vsIndex
  type: integer
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/f5-virtual-server-schema.json
slug: f5-virtual-server
source_filename: f5-virtual-server-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.f5.com/bigip/ltm/virtual-server\",\n  \"title\": \"F5 BIG-IP Virtual Server\",\n  \"description\": \"Schema for an F5 BIG-IP LTM virtual server resource that directs client traffic to pools of backend servers based on IP address, port, and protocol configuration. Virtual servers are the core traffic management objects in the BIG-IP Local Traffic Manager.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"destination\"\n  ],\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"tm:ltm:virtual:virtualstate\",\n      \"description\": \"Resource type identifier for a virtual server.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the virtual server resource within its partition.\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"pattern\": \"^[a-zA-Z0-9_.\\\
  \\-]+$\",\n      \"examples\": [\n        \"my_virtual_server\",\n        \"web_app_vs\",\n        \"api_gateway_443\"\n      ]\n    },\n    \"fullPath\": {\n      \"type\": \"string\",\n      \"description\": \"Full administrative path including partition (e.g., /Common/my_virtual).\",\n      \"pattern\": \"^/[a-zA-Z0-9_.\\\\-]+/[a-zA-Z0-9_.\\\\-]+$\",\n      \"readOnly\": true,\n      \"examples\": [\n        \"/Common/my_virtual_server\"\n      ]\n    },\n    \"generation\": {\n      \"type\": \"integer\",\n      \"description\": \"Configuration generation counter incremented on each change.\",\n      \"minimum\": 0,\n      \"readOnly\": true\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Self-referencing URI for this virtual server resource.\",\n      \"readOnly\": true\n    },\n    \"addressStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the virtual contributes to the operational status of\
  \ the associated virtual address.\",\n      \"enum\": [\n        \"yes\",\n        \"no\"\n      ],\n      \"default\": \"yes\"\n    },\n    \"autoLasthop\": {\n      \"type\": \"string\",\n      \"description\": \"Automatic last hop setting controlling return traffic routing when the BIG-IP is not the default gateway.\",\n      \"enum\": [\n        \"default\",\n        \"enabled\",\n        \"disabled\"\n      ],\n      \"default\": \"default\"\n    },\n    \"cmpEnabled\": {\n      \"type\": \"string\",\n      \"description\": \"Whether Clustered Multi-Processing (CMP) acceleration is enabled for this virtual server.\",\n      \"enum\": [\n        \"yes\",\n        \"no\"\n      ],\n      \"default\": \"yes\"\n    },\n    \"connectionLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of concurrent connections allowed for this virtual server. A value of 0 means unlimited connections.\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"description\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"User-defined description of the virtual server and its purpose.\",\n      \"maxLength\": 1024\n    },\n    \"destination\": {\n      \"type\": \"string\",\n      \"description\": \"Destination IP address and service port the virtual server listens on, specified in /partition/address:port or /partition/address.port format.\",\n      \"examples\": [\n        \"/Common/10.0.0.100:80\",\n        \"/Common/10.0.0.100:443\",\n        \"/Common/192.168.1.100.https\"\n      ]\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, the virtual server does not accept new connections. Existing connections are maintained.\",\n      \"default\": false\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, the virtual server accepts and processes client traffic.\",\n      \"default\": true\n    },\n    \"fallbackPersistence\": {\n      \"type\": \"string\",\n   \
  \   \"description\": \"Persistence profile to use as a fallback when the primary persistence method fails to establish a session.\",\n      \"examples\": [\n        \"/Common/source_addr\"\n      ]\n    },\n    \"gtmScore\": {\n      \"type\": \"integer\",\n      \"description\": \"Score value used by the Global Traffic Manager for load balancing decisions across data centers.\",\n      \"minimum\": 0,\n      \"default\": 0\n    },\n    \"ipProtocol\": {\n      \"type\": \"string\",\n      \"description\": \"Network protocol the virtual server handles.\",\n      \"enum\": [\n        \"tcp\",\n        \"udp\",\n        \"sctp\",\n        \"any\"\n      ],\n      \"examples\": [\n        \"tcp\"\n      ]\n    },\n    \"mask\": {\n      \"type\": \"string\",\n      \"description\": \"Network mask for the destination address. Use 255.255.255.255 for a host-specific virtual server or a subnet mask for a network virtual server.\",\n      \"format\": \"ipv4\",\n      \"default\": \"255.255.255.255\"\
  ,\n      \"examples\": [\n        \"255.255.255.255\",\n        \"255.255.255.0\"\n      ]\n    },\n    \"mirror\": {\n      \"type\": \"string\",\n      \"description\": \"Whether connection and persistence state mirroring is enabled for high-availability failover scenarios.\",\n      \"enum\": [\n        \"enabled\",\n        \"disabled\"\n      ],\n      \"default\": \"disabled\"\n    },\n    \"nat64\": {\n      \"type\": \"string\",\n      \"description\": \"Whether NAT64 IPv6-to-IPv4 address translation is enabled.\",\n      \"enum\": [\n        \"enabled\",\n        \"disabled\"\n      ],\n      \"default\": \"disabled\"\n    },\n    \"partition\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative partition containing this virtual server resource.\",\n      \"default\": \"Common\",\n      \"examples\": [\n        \"Common\",\n        \"Production\",\n        \"Staging\"\n      ]\n    },\n    \"persist\": {\n      \"type\": \"array\",\n      \"description\":\
  \ \"Persistence profiles applied to the virtual server for maintaining session affinity.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PersistenceReference\"\n      }\n    },\n    \"pool\": {\n      \"type\": \"string\",\n      \"description\": \"Default pool that receives traffic from this virtual server, specified as a full partition-qualified path.\",\n      \"examples\": [\n        \"/Common/my_pool\",\n        \"/Common/web_pool\"\n      ]\n    },\n    \"profiles\": {\n      \"type\": \"array\",\n      \"description\": \"Traffic processing profiles applied to this virtual server (e.g., HTTP, TCP, SSL profiles).\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ProfileReference\"\n      }\n    },\n    \"rateLimit\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum number of new connections per second. A value of 'disabled' or '0' means no rate limiting.\",\n      \"default\": \"disabled\"\n    },\n    \"rateLimitMode\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Scope at which rate limiting is applied.\",\n      \"enum\": [\n        \"object\",\n        \"object-source\",\n        \"object-destination\",\n        \"object-source-destination\"\n      ],\n      \"default\": \"object\"\n    },\n    \"rateLimitDstMask\": {\n      \"type\": \"integer\",\n      \"description\": \"Destination address mask bits used for rate limit tracking.\",\n      \"minimum\": 0,\n      \"maximum\": 32,\n      \"default\": 0\n    },\n    \"rateLimitSrcMask\": {\n      \"type\": \"integer\",\n      \"description\": \"Source address mask bits used for rate limit tracking.\",\n      \"minimum\": 0,\n      \"maximum\": 32,\n      \"default\": 0\n    },\n    \"rules\": {\n      \"type\": \"array\",\n      \"description\": \"iRules applied to this virtual server for custom traffic processing logic.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\n          \"/Common/my_irule\",\n          \"/Common/redirect_http\"\
  \n        ]\n      ]\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source address filter. Only connections from this network are accepted by the virtual server.\",\n      \"default\": \"0.0.0.0/0\",\n      \"examples\": [\n        \"0.0.0.0/0\",\n        \"10.0.0.0/8\"\n      ]\n    },\n    \"sourcePort\": {\n      \"type\": \"string\",\n      \"description\": \"Source port translation behavior controlling how client source ports are handled.\",\n      \"enum\": [\n        \"preserve\",\n        \"preserve-strict\",\n        \"change\"\n      ],\n      \"default\": \"preserve\"\n    },\n    \"synCookieStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current SYN Cookie DDoS protection status.\",\n      \"enum\": [\n        \"not-activated\",\n        \"activated\"\n      ],\n      \"readOnly\": true\n    },\n    \"translateAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Whether destination address translation is enabled.\
  \ When enabled, the BIG-IP translates the destination address to the pool member address.\",\n      \"enum\": [\n        \"enabled\",\n        \"disabled\"\n      ],\n      \"default\": \"enabled\"\n    },\n    \"translatePort\": {\n      \"type\": \"string\",\n      \"description\": \"Whether destination port translation is enabled. When enabled, the BIG-IP translates the destination port to the pool member port.\",\n      \"enum\": [\n        \"enabled\",\n        \"disabled\"\n      ],\n      \"default\": \"enabled\"\n    },\n    \"vlansEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, the virtual server is enabled only on VLANs listed in the vlans property.\"\n    },\n    \"vlansDisabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"When true, the virtual server is disabled on VLANs listed in the vlans property.\"\n    },\n    \"vlans\": {\n      \"type\": \"array\",\n      \"description\": \"List of VLANs on which the virtual server is\
  \ enabled or disabled, depending on vlansEnabled/vlansDisabled setting.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\n          \"/Common/external\",\n          \"/Common/internal\"\n        ]\n      ]\n    },\n    \"vsIndex\": {\n      \"type\": \"integer\",\n      \"description\": \"System-assigned index for the virtual server.\",\n      \"readOnly\": true,\n      \"minimum\": 0\n    }\n  },\n  \"$defs\": {\n    \"PersistenceReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a persistence profile applied to a virtual server.\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the persistence profile.\",\n          \"examples\": [\n            \"cookie\",\n            \"source_addr\",\n            \"ssl\",\n            \"hash\"\n          ]\n        },\n        \"tmDefault\": {\n     \
  \     \"type\": \"string\",\n          \"description\": \"Whether this is the default persistence profile for the virtual server.\",\n          \"enum\": [\n            \"yes\",\n            \"no\"\n          ]\n        }\n      }\n    },\n    \"ProfileReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a traffic processing profile applied to a virtual server.\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the profile.\",\n          \"examples\": [\n            \"http\",\n            \"tcp\",\n            \"clientssl\",\n            \"serverssl\",\n            \"udp\",\n            \"fastL4\"\n          ]\n        },\n        \"context\": {\n          \"type\": \"string\",\n          \"description\": \"Connection side to which the profile applies.\",\n          \"enum\": [\n            \"all\",\n            \"clientside\",\n        \
  \    \"serverside\"\n          ],\n          \"default\": \"all\"\n        },\n        \"fullPath\": {\n          \"type\": \"string\",\n          \"description\": \"Full partition-qualified path to the profile.\",\n          \"examples\": [\n            \"/Common/http\",\n            \"/Common/tcp\",\n            \"/Common/clientssl\"\n          ]\n        }\n      }\n    },\n    \"Pool\": {\n      \"type\": \"object\",\n      \"description\": \"A load balancing pool containing backend server members.\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"const\": \"tm:ltm:pool:poolstate\",\n          \"readOnly\": true\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the pool resource.\",\n          \"minLength\": 1,\n          \"maxLength\": 255\n        },\n        \"fullPath\": {\n          \"type\": \"string\",\n          \"readOnly\":\
  \ true\n        },\n        \"generation\": {\n          \"type\": \"integer\",\n          \"readOnly\": true\n        },\n        \"selfLink\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"readOnly\": true\n        },\n        \"allowNat\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the pool can load balance NAT connections.\",\n          \"enum\": [\"yes\", \"no\"],\n          \"default\": \"yes\"\n        },\n        \"allowSnat\": {\n          \"type\": \"string\",\n          \"description\": \"Whether the pool can load balance SNAT connections.\",\n          \"enum\": [\"yes\", \"no\"],\n          \"default\": \"yes\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"User-defined description.\"\n        },\n        \"loadBalancingMode\": {\n          \"type\": \"string\",\n          \"description\": \"Load balancing algorithm used to distribute traffic across pool\
  \ members.\",\n          \"enum\": [\n            \"round-robin\",\n            \"ratio-member\",\n            \"least-connections-member\",\n            \"observed-member\",\n            \"predictive-member\",\n            \"ratio-node\",\n            \"least-connections-node\",\n            \"fastest-node\",\n            \"observed-node\",\n            \"predictive-node\",\n            \"dynamic-ratio-node\",\n            \"fastest-app-response\",\n            \"least-sessions\",\n            \"dynamic-ratio-member\",\n            \"weighted-least-connections-member\",\n            \"weighted-least-connections-node\",\n            \"ratio-session\",\n            \"ratio-least-connections-member\",\n            \"ratio-least-connections-node\"\n          ],\n          \"default\": \"round-robin\"\n        },\n        \"minActiveMembers\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum number of active members before priority-group activation.\",\n          \"\
  minimum\": 0,\n          \"default\": 0\n        },\n        \"monitor\": {\n          \"type\": \"string\",\n          \"description\": \"Health monitor(s) applied to pool members.\"\n        },\n        \"partition\": {\n          \"type\": \"string\",\n          \"default\": \"Common\"\n        },\n        \"reselectTries\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of reselection attempts after a passive failure detection.\",\n          \"minimum\": 0,\n          \"default\": 0\n        },\n        \"serviceDownAction\": {\n          \"type\": \"string\",\n          \"description\": \"Action taken when all pool members are unavailable.\",\n          \"enum\": [\"none\", \"reset\", \"reselect\", \"drop\"],\n          \"default\": \"none\"\n        },\n        \"slowRampTime\": {\n          \"type\": \"integer\",\n          \"description\": \"Time in seconds to gradually ramp up traffic to newly enabled members.\",\n          \"minimum\": 0,\n         \
  \ \"default\": 10\n        }\n      }\n    },\n    \"PoolMember\": {\n      \"type\": \"object\",\n      \"description\": \"An individual backend server member within a pool.\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"const\": \"tm:ltm:pool:members:membersstate\",\n          \"readOnly\": true\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Member name in address:port format.\",\n          \"pattern\": \"^[\\\\w.\\\\-]+:\\\\d+$\",\n          \"examples\": [\"10.0.0.1:80\", \"web-server-01:443\"]\n        },\n        \"fullPath\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"IP address of the pool member.\",\n          \"format\": \"ipv4\"\n        },\n        \"connectionLimit\": {\n          \"type\": \"integer\",\n   \
  \       \"description\": \"Maximum concurrent connections. 0 means unlimited.\",\n          \"minimum\": 0,\n          \"default\": 0\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"dynamicRatio\": {\n          \"type\": \"integer\",\n          \"description\": \"Dynamic ratio weight for load balancing.\",\n          \"default\": 1\n        },\n        \"monitor\": {\n          \"type\": \"string\",\n          \"description\": \"Health monitor override for this specific member.\",\n          \"default\": \"default\"\n        },\n        \"partition\": {\n          \"type\": \"string\",\n          \"default\": \"Common\"\n        },\n        \"priorityGroup\": {\n          \"type\": \"integer\",\n          \"description\": \"Priority group number. Higher values receive traffic first.\",\n          \"minimum\": 0,\n          \"default\": 0\n        },\n        \"rateLimit\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum\
  \ connections per second.\",\n          \"default\": \"disabled\"\n        },\n        \"ratio\": {\n          \"type\": \"integer\",\n          \"description\": \"Ratio weight for proportional load balancing.\",\n          \"minimum\": 1,\n          \"default\": 1\n        },\n        \"session\": {\n          \"type\": \"string\",\n          \"description\": \"Session availability state.\",\n          \"enum\": [\"user-enabled\", \"user-disabled\", \"monitor-enabled\"],\n          \"default\": \"user-enabled\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"description\": \"Operational state of the member.\",\n          \"enum\": [\"user-up\", \"user-down\", \"up\", \"down\", \"unchecked\"]\n        }\n      }\n    },\n    \"Node\": {\n      \"type\": \"object\",\n      \"description\": \"A backend server node identified by IP address or FQDN.\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"kind\": {\n        \
  \  \"type\": \"string\",\n          \"const\": \"tm:ltm:node:nodestate\",\n          \"readOnly\": true\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the node, typically its IP address.\",\n          \"examples\": [\"10.0.0.1\", \"web-server-01\"]\n        },\n        \"fullPath\": {\n          \"type\": \"string\",\n          \"readOnly\": true\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"IP address of the node.\",\n          \"format\": \"ipv4\"\n        },\n        \"connectionLimit\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"default\": 0\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"dynamicRatio\": {\n          \"type\": \"integer\",\n          \"default\": 1\n        },\n        \"fqdn\": {\n          \"$ref\": \"#/$defs/NodeFqdn\"\n        },\n        \"logging\": {\n          \"type\":\
  \ \"string\",\n          \"description\": \"Whether monitor actions are logged.\",\n          \"enum\": [\"enabled\", \"disabled\"],\n          \"default\": \"disabled\"\n        },\n        \"monitor\": {\n          \"type\": \"string\",\n          \"description\": \"Health monitor applied to the node.\",\n          \"default\": \"default\"\n        },\n        \"partition\": {\n          \"type\": \"string\",\n          \"default\": \"Common\"\n        },\n        \"rateLimit\": {\n          \"type\": \"string\",\n          \"default\": \"disabled\"\n        },\n        \"ratio\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"default\": 1\n        },\n        \"session\": {\n          \"type\": \"string\",\n          \"enum\": [\"user-enabled\", \"user-disabled\", \"monitor-enabled\"],\n          \"default\": \"user-enabled\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"enum\": [\"user-up\", \"user-down\", \"up\", \"down\"\
  , \"unchecked\"]\n        }\n      }\n    },\n    \"NodeFqdn\": {\n      \"type\": \"object\",\n      \"description\": \"FQDN configuration for DNS-based node address resolution.\",\n      \"properties\": {\n        \"addressFamily\": {\n          \"type\": \"string\",\n          \"description\": \"IP address family for DNS resolution.\",\n          \"enum\": [\"ipv4\", \"ipv6\"],\n          \"default\": \"ipv4\"\n        },\n        \"autopopulate\": {\n          \"type\": \"string\",\n          \"description\": \"Whether to auto-populate the node with all addresses from DNS lookup.\",\n          \"enum\": [\"enabled\", \"disabled\"],\n          \"default\": \"disabled\"\n        },\n        \"downInterval\": {\n          \"type\": \"integer\",\n          \"description\": \"Interval in seconds for DNS queries when the node is marked down.\",\n          \"minimum\": 0,\n          \"default\": 5\n        },\n        \"interval\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Interval in seconds between DNS queries.\",\n          \"default\": \"3600\"\n        },\n        \"tmName\": {\n          \"type\": \"string\",\n          \"description\": \"The fully qualified domain name to resolve.\",\n          \"format\": \"hostname\"\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"name\": \"web_app_vs\",\n      \"partition\": \"Common\",\n      \"destination\": \"/Common/10.0.0.100:443\",\n      \"description\": \"Production web application virtual server with SSL offloading\",\n      \"ipProtocol\": \"tcp\",\n      \"mask\": \"255.255.255.255\",\n      \"pool\": \"/Common/web_pool\",\n      \"source\": \"0.0.0.0/0\",\n      \"sourcePort\": \"preserve\",\n      \"translateAddress\": \"enabled\",\n      \"translatePort\": \"enabled\",\n      \"profiles\": [\n        {\n          \"name\": \"tcp\",\n          \"context\": \"all\"\n        },\n        {\n          \"name\": \"http\",\n          \"context\": \"all\"\n        },\n        {\n \
  \         \"name\": \"clientssl\",\n          \"context\": \"clientside\"\n        }\n      ],\n      \"persist\": [\n        {\n          \"name\": \"cookie\",\n          \"tmDefault\": \"yes\"\n        }\n      ],\n      \"vlansEnabled\": true,\n      \"vlans\": [\n        \"/Common/external\"\n      ]\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/f5-virtual-server-schema.json
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
title: F5 BIG-IP Virtual Server
---
