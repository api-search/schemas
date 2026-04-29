---
description: Attributes of a NetBackup client host
layout: schema
name: ClientAttributes
properties_list:
- description: Fully qualified hostname of the client
  name: hostName
  type: string
- description: Type of host in the NetBackup environment
  name: hostType
  type: string
- description: Operating system of the client
  name: os
  type: string
- description: Hardware platform of the client
  name: platform
  type: string
- description: NetBackup client software version
  name: version
  type: string
- description: SHA-256 fingerprint of the client certificate
  name: fingerprintSha256
  type: string
- description: Trust level established with the primary server
  name: trustLevel
  type: string
- description: Current communication status
  name: communicationStatus
  type: string
- description: Timestamp of the last successful communication
  name: lastConnectedTime
  type: string
provider_name: Veritas NetBackup
provider_slug: veritas-netbackup
schema_file: json-schema/veritas-netbackup-rest-client-attributes-schema.json
slug: veritas-netbackup-rest-client-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClientAttributes\",\n  \"type\": \"object\",\n  \"description\": \"Attributes of a NetBackup client host\",\n  \"properties\": {\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified hostname of the client\"\n    },\n    \"hostType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of host in the NetBackup environment\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system of the client\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware platform of the client\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"NetBackup client software version\"\n    },\n    \"fingerprintSha256\": {\n      \"type\": \"string\",\n      \"description\": \"SHA-256 fingerprint of the client certificate\"\n    },\n    \"trustLevel\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Trust level established with the primary server\"\n    },\n    \"communicationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current communication status\"\n    },\n    \"lastConnectedTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the last successful communication\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veritas-netbackup/refs/heads/main/json-schema/veritas-netbackup-rest-client-attributes-schema.json
tags:
- Backup
- Data Protection
- Disaster Recovery
- Enterprise
- Recovery
- Storage
title: ClientAttributes
---
