---
description: Represents a client (server, workstation, virtual machine, or laptop) registered with the Commvault CommServe for data protection. Clients host agents that perform backup and restore operations.
layout: schema
name: Commvault Client
properties_list:
- description: Unique identifier for the client
  name: clientId
  type: integer
- description: Display name of the client
  name: clientName
  type: string
- description: Network hostname or FQDN of the client
  name: hostName
  type: string
- description: User-friendly display name
  name: displayName
  type: string
- description: Operating system type of the client
  name: osType
  type: string
- description: Detailed operating system version string
  name: osVersion
  type: string
- description: CommCell ID the client belongs to
  name: commCellId
  type: integer
- description: Type of client
  name: clientType
  type: string
- description: Controls which operations are enabled on this client
  name: activityControl
  type: object
- description: List of installed agents (iDataAgents) on this client
  name: agents
  type: array
- description: Path to the Commvault software installation directory
  name: installDirectory
  type: string
- description: Timestamp of the last successful backup on this client
  name: lastBackupTime
  type: string
- description: Name of the server plan associated with this client
  name: planName
  type: string
provider_name: Commvault
provider_slug: commvault
schema_file: json-schema/commvault-client-schema.json
slug: commvault-client
source_filename: commvault-client-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.commvault.com/schemas/commvault/client.json\",\n  \"title\": \"Commvault Client\",\n  \"description\": \"Represents a client (server, workstation, virtual machine, or laptop) registered with the Commvault CommServe for data protection. Clients host agents that perform backup and restore operations.\",\n  \"type\": \"object\",\n  \"required\": [\"clientId\", \"clientName\"],\n  \"properties\": {\n    \"clientId\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the client\"\n    },\n    \"clientName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the client\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"Network hostname or FQDN of the client\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"User-friendly\
  \ display name\"\n    },\n    \"osType\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system type of the client\",\n      \"enum\": [\"Windows\", \"Linux\", \"Unix\", \"macOS\", \"FreeBSD\"]\n    },\n    \"osVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed operating system version string\"\n    },\n    \"commCellId\": {\n      \"type\": \"integer\",\n      \"description\": \"CommCell ID the client belongs to\"\n    },\n    \"clientType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of client\",\n      \"enum\": [\n        \"Server\",\n        \"Workstation\",\n        \"Laptop\",\n        \"VirtualMachine\",\n        \"MediaAgent\",\n        \"ProxyServer\",\n        \"NASClient\"\n      ]\n    },\n    \"activityControl\": {\n      \"type\": \"object\",\n      \"description\": \"Controls which operations are enabled on this client\",\n      \"properties\": {\n        \"enableBackup\": {\n          \"type\": \"boolean\"\
  ,\n          \"description\": \"Whether backup operations are enabled\"\n        },\n        \"enableRestore\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether restore operations are enabled\"\n        },\n        \"enableDataAging\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether data aging operations are enabled\"\n        }\n      }\n    },\n    \"agents\": {\n      \"type\": \"array\",\n      \"description\": \"List of installed agents (iDataAgents) on this client\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Agent\"\n      }\n    },\n    \"installDirectory\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the Commvault software installation directory\"\n    },\n    \"lastBackupTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last successful backup on this client\"\n    },\n    \"planName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Name of the server plan associated with this client\"\n    }\n  },\n  \"$defs\": {\n    \"Agent\": {\n      \"type\": \"object\",\n      \"description\": \"An iDataAgent installed on a client that handles backup and restore for a specific application type\",\n      \"properties\": {\n        \"applicationId\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique application type identifier\"\n        },\n        \"applicationName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the agent (e.g., File System, SQL Server, Exchange)\"\n        },\n        \"installed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the agent is currently installed\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Agent software version\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/commvault/refs/heads/main/json-schema/commvault-client-schema.json
tags:
- Backup
- Cloud Storage
- Cyber Recovery
- Data Management
- Data Protection
- Disaster Recovery
- Enterprise Software
title: Commvault Client
---
