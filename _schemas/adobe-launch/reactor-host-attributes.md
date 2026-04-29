---
description: ''
layout: schema
name: HostAttributes
properties_list:
- description: The human-readable name of the host.
  name: name
  type: string
- description: The hosting type.
  name: type_of
  type: string
- description: The host URL for SFTP hosts.
  name: server
  type: string
- description: The server port for SFTP hosts.
  name: port
  type: integer
- description: The URL path suffix for SFTP hosts.
  name: path
  type: string
- description: The authentication username for SFTP hosts.
  name: username
  type: string
- description: The encrypted private key for SFTP hosts.
  name: encrypted_private_key
  type: string
- description: Whether to use file copying instead of symbolic links for SFTP hosts.
  name: skip_symlinks
  type: boolean
- description: The current status of the host.
  name: status
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-host-attributes-schema.json
slug: reactor-host-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HostAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the host.\"\n    },\n    \"type_of\": {\n      \"type\": \"string\",\n      \"description\": \"The hosting type.\"\n    },\n    \"server\": {\n      \"type\": \"string\",\n      \"description\": \"The host URL for SFTP hosts.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The server port for SFTP hosts.\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"The URL path suffix for SFTP hosts.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication username for SFTP hosts.\"\n    },\n    \"encrypted_private_key\": {\n      \"type\": \"string\",\n      \"description\": \"The encrypted private key for SFTP hosts.\"\n    },\n\
  \    \"skip_symlinks\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to use file copying instead of symbolic links for SFTP hosts.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the host.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-host-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: HostAttributes
---
