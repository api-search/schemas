---
description: Represents a managed endpoint (computer, server, or device) in the Tanium platform. Endpoints are the primary entities that Tanium discovers, monitors, and manages across the enterprise.
layout: schema
name: Tanium Endpoint
properties_list:
- description: Unique numeric identifier for the endpoint in Tanium
  name: id
  type: integer
- description: Hostname of the endpoint
  name: computerName
  type: string
- description: Tanium client identifier assigned to the endpoint
  name: computerID
  type: string
- description: Primary IP address of the endpoint
  name: ipAddress
  type: string
- description: All IP addresses associated with the endpoint
  name: ipAddresses
  type: array
- description: Primary MAC address of the endpoint
  name: macAddress
  type: string
- description: Full operating system name and version
  name: operatingSystem
  type: string
- description: Operating system platform category
  name: osPlatform
  type: string
- description: Hardware manufacturer
  name: manufacturer
  type: string
- description: Hardware model
  name: model
  type: string
- description: Hardware serial number
  name: serialNumber
  type: string
- description: Active Directory or DNS domain name
  name: domainName
  type: string
- description: Timestamp of the last client registration with the Tanium server
  name: lastRegistration
  type: string
- description: Version of the Tanium client installed on the endpoint
  name: taniumClientVersion
  type: string
- description: Whether the endpoint is a virtual machine
  name: isVirtual
  type: boolean
- description: Physical chassis type (Desktop, Laptop, Server, Virtual)
  name: chassisType
  type: string
- description: Total physical memory
  name: totalMemory
  type: string
- description: Total disk space
  name: diskSpace
  type: string
- description: Available free disk space
  name: freeDiskSpace
  type: string
- description: List of installed software applications
  name: installedApplications
  type: array
- description: Tags assigned to the endpoint for organization
  name: tags
  type: array
provider_name: Tanium
provider_slug: tanium
schema_file: json-schema/tanium-endpoint-schema.json
slug: tanium-endpoint
source_filename: tanium-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/tanium/blob/main/json-schema/tanium-endpoint-schema.json\",\n  \"title\": \"Tanium Endpoint\",\n  \"description\": \"Represents a managed endpoint (computer, server, or device) in the Tanium platform. Endpoints are the primary entities that Tanium discovers, monitors, and manages across the enterprise.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for the endpoint in Tanium\"\n    },\n    \"computerName\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the endpoint\"\n    },\n    \"computerID\": {\n      \"type\": \"string\",\n      \"description\": \"Tanium client identifier assigned to the endpoint\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Primary IP address of the endpoint\"\n    },\n    \"ipAddresses\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"All IP addresses associated with the endpoint\"\n    },\n    \"macAddress\": {\n      \"type\": \"string\",\n      \"description\": \"Primary MAC address of the endpoint\"\n    },\n    \"operatingSystem\": {\n      \"type\": \"string\",\n      \"description\": \"Full operating system name and version\"\n    },\n    \"osPlatform\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system platform category\",\n      \"enum\": [\"Windows\", \"Linux\", \"Mac\", \"Solaris\", \"AIX\"]\n    },\n    \"manufacturer\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware manufacturer\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware model\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware serial number\"\n    },\n    \"domainName\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Active Directory or DNS domain name\"\n    },\n    \"lastRegistration\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last client registration with the Tanium server\"\n    },\n    \"taniumClientVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the Tanium client installed on the endpoint\"\n    },\n    \"isVirtual\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the endpoint is a virtual machine\"\n    },\n    \"chassisType\": {\n      \"type\": \"string\",\n      \"description\": \"Physical chassis type (Desktop, Laptop, Server, Virtual)\"\n    },\n    \"totalMemory\": {\n      \"type\": \"string\",\n      \"description\": \"Total physical memory\"\n    },\n    \"diskSpace\": {\n      \"type\": \"string\",\n      \"description\": \"Total disk space\"\n    },\n    \"freeDiskSpace\": {\n      \"type\": \"string\",\n      \"description\": \"Available\
  \ free disk space\"\n    },\n    \"installedApplications\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Application name\"\n          },\n          \"version\": {\n            \"type\": \"string\",\n            \"description\": \"Application version\"\n          },\n          \"vendor\": {\n            \"type\": \"string\",\n            \"description\": \"Application vendor\"\n          }\n        }\n      },\n      \"description\": \"List of installed software applications\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags assigned to the endpoint for organization\"\n    }\n  },\n  \"required\": [\"computerName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tanium/refs/heads/main/json-schema/tanium-endpoint-schema.json
tags:
- Compliance
- Endpoint Management
- Patch Management
- Security
- Threat Detection
- Unified Endpoint Management
title: Tanium Endpoint
---
