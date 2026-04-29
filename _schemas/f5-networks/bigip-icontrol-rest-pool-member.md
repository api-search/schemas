---
description: A pool member resource representing an individual backend server within a pool, identified by address and port.
layout: schema
name: PoolMember
properties_list:
- description: Resource type identifier.
  name: kind
  type: string
- description: Member name in address:port format.
  name: name
  type: string
- description: Full path including partition.
  name: fullPath
  type: string
- description: ''
  name: generation
  type: integer
- description: ''
  name: selfLink
  type: string
- description: IP address of the pool member.
  name: address
  type: string
- description: Maximum concurrent connections. 0 means unlimited.
  name: connectionLimit
  type: integer
- description: User-defined description.
  name: description
  type: string
- description: Dynamic ratio for load balancing.
  name: dynamicRatio
  type: integer
- description: Whether this is a transient auto-discovered member.
  name: ephemeral
  type: string
- description: Whether the member inherits the encapsulation profile from its parent pool.
  name: inheritProfile
  type: string
- description: Whether monitor actions are logged.
  name: logging
  type: string
- description: Health monitor override for this member.
  name: monitor
  type: string
- description: Administrative partition.
  name: partition
  type: string
- description: Priority group number. Higher values receive traffic first when priority-group activation is configured.
  name: priorityGroup
  type: integer
- description: Maximum connections per second. disabled means no limit.
  name: rateLimit
  type: string
- description: Ratio weight for load balancing.
  name: ratio
  type: integer
- description: Session availability state.
  name: session
  type: string
- description: Operational state of the member.
  name: state
  type: string
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-pool-member-schema.json
slug: bigip-icontrol-rest-pool-member
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PoolMember\",\n  \"type\": \"object\",\n  \"description\": \"A pool member resource representing an individual backend server within a pool, identified by address and port.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Member name in address:port format.\"\n    },\n    \"fullPath\": {\n      \"type\": \"string\",\n      \"description\": \"Full path including partition.\"\n    },\n    \"generation\": {\n      \"type\": \"integer\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the pool member.\"\n    },\n    \"connectionLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum concurrent connections. 0 means unlimited.\"\
  \n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined description.\"\n    },\n    \"dynamicRatio\": {\n      \"type\": \"integer\",\n      \"description\": \"Dynamic ratio for load balancing.\"\n    },\n    \"ephemeral\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this is a transient auto-discovered member.\"\n    },\n    \"inheritProfile\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the member inherits the encapsulation profile from its parent pool.\"\n    },\n    \"logging\": {\n      \"type\": \"string\",\n      \"description\": \"Whether monitor actions are logged.\"\n    },\n    \"monitor\": {\n      \"type\": \"string\",\n      \"description\": \"Health monitor override for this member.\"\n    },\n    \"partition\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative partition.\"\n    },\n    \"priorityGroup\": {\n      \"type\": \"integer\",\n      \"description\": \"Priority\
  \ group number. Higher values receive traffic first when priority-group activation is configured.\"\n    },\n    \"rateLimit\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum connections per second. disabled means no limit.\"\n    },\n    \"ratio\": {\n      \"type\": \"integer\",\n      \"description\": \"Ratio weight for load balancing.\"\n    },\n    \"session\": {\n      \"type\": \"string\",\n      \"description\": \"Session availability state.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Operational state of the member.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-pool-member-schema.json
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
title: PoolMember
---
