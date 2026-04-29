---
description: A node resource representing an individual backend server by its IP address or FQDN. Nodes are automatically created when pool members are added, or can be created independently.
layout: schema
name: Node
properties_list:
- description: Resource type identifier.
  name: kind
  type: string
- description: Name of the node (typically the IP address).
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
- description: IP address of the node.
  name: address
  type: string
- description: Maximum concurrent connections. 0 means unlimited.
  name: connectionLimit
  type: integer
- description: User-defined description.
  name: description
  type: string
- description: Dynamic ratio weight for load balancing.
  name: dynamicRatio
  type: integer
- description: Whether this is a transient auto-discovered node.
  name: ephemeral
  type: string
- description: FQDN configuration for DNS-based node resolution.
  name: fqdn
  type: object
- description: Whether monitor actions are logged.
  name: logging
  type: string
- description: Health monitor applied to the node.
  name: monitor
  type: string
- description: Administrative partition.
  name: partition
  type: string
- description: Maximum connections per second. 0 means no limit.
  name: rateLimit
  type: string
- description: Fixed ratio weight for load balancing.
  name: ratio
  type: integer
- description: Session availability state.
  name: session
  type: string
- description: Operational state of the node.
  name: state
  type: string
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-node-schema.json
slug: bigip-icontrol-rest-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Node\",\n  \"type\": \"object\",\n  \"description\": \"A node resource representing an individual backend server by its IP address or FQDN. Nodes are automatically created when pool members are added, or can be created independently.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the node (typically the IP address).\"\n    },\n    \"fullPath\": {\n      \"type\": \"string\",\n      \"description\": \"Full path including partition.\"\n    },\n    \"generation\": {\n      \"type\": \"integer\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the node.\"\n    },\n    \"connectionLimit\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Maximum concurrent connections. 0 means unlimited.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-defined description.\"\n    },\n    \"dynamicRatio\": {\n      \"type\": \"integer\",\n      \"description\": \"Dynamic ratio weight for load balancing.\"\n    },\n    \"ephemeral\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this is a transient auto-discovered node.\"\n    },\n    \"fqdn\": {\n      \"type\": \"object\",\n      \"description\": \"FQDN configuration for DNS-based node resolution.\"\n    },\n    \"logging\": {\n      \"type\": \"string\",\n      \"description\": \"Whether monitor actions are logged.\"\n    },\n    \"monitor\": {\n      \"type\": \"string\",\n      \"description\": \"Health monitor applied to the node.\"\n    },\n    \"partition\": {\n      \"type\": \"string\",\n      \"description\": \"Administrative partition.\"\n    },\n    \"rateLimit\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Maximum connections per second. 0 means no limit.\"\n    },\n    \"ratio\": {\n      \"type\": \"integer\",\n      \"description\": \"Fixed ratio weight for load balancing.\"\n    },\n    \"session\": {\n      \"type\": \"string\",\n      \"description\": \"Session availability state.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Operational state of the node.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-node-schema.json
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
title: Node
---
