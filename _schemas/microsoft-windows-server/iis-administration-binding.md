---
description: Defines the protocol, IP address, port, and optional hostname that a web site listens on. The binding_information property format is '{ip_address}:{port}:{hostname}' for HTTP and HTTPS protocols.
layout: schema
name: Binding
properties_list:
- description: The protocol for this binding (e.g., http, https, net.tcp).
  name: protocol
  type: string
- description: Combined binding string in the format '{ip_address}:{port}:{hostname}'.
  name: binding_information
  type: string
- description: The IP address to bind to. Use '*' for all addresses.
  name: ip_address
  type: string
- description: The port number to listen on.
  name: port
  type: integer
- description: The hostname for host header-based routing.
  name: hostname
  type: string
- description: Whether Server Name Indication (SNI) is required for this binding.
  name: require_sni
  type: boolean
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-binding-schema.json
slug: iis-administration-binding
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Binding\",\n  \"type\": \"object\",\n  \"description\": \"Defines the protocol, IP address, port, and optional hostname that a web site listens on. The binding_information property format is '{ip_address}:{port}:{hostname}' for HTTP and HTTPS protocols.\",\n  \"properties\": {\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"The protocol for this binding (e.g., http, https, net.tcp).\"\n    },\n    \"binding_information\": {\n      \"type\": \"string\",\n      \"description\": \"Combined binding string in the format '{ip_address}:{port}:{hostname}'.\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address to bind to. Use '*' for all addresses.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number to listen on.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"The hostname for host header-based routing.\"\n    },\n    \"require_sni\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Server Name Indication (SNI) is required for this binding.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-binding-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: Binding
---
