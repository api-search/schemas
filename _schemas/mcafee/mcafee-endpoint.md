---
description: A managed endpoint (system) registered in McAfee ePO or MVISION, representing a computer, server, or device with McAfee security products installed and managed through the centralized console.
layout: schema
name: McAfee Managed Endpoint
properties_list:
- description: Unique McAfee Agent GUID identifying the endpoint
  name: agentGuid
  type: string
- description: NetBIOS or hostname of the endpoint
  name: computerName
  type: string
- description: Primary IPv4 address of the endpoint
  name: ipAddress
  type: string
- description: IPv6 address of the endpoint
  name: ipv6Address
  type: string
- description: MAC address of the primary network adapter
  name: macAddress
  type: string
- description: ''
  name: operatingSystem
  type: object
- description: Active Directory domain or workgroup name
  name: domainName
  type: string
- description: Currently logged-in user name
  name: userName
  type: string
- description: Installed McAfee Agent version
  name: agentVersion
  type: string
- description: Management state of the McAfee Agent
  name: agentStatus
  type: string
- description: Timestamp of the last agent-server communication
  name: lastCommunication
  type: string
- description: Full path in the ePO System Tree (e.g., My Organization/Workstations/Finance)
  name: systemGroupPath
  type: string
- description: Tags applied to this endpoint in ePO
  name: tags
  type: array
- description: McAfee security products installed on the endpoint
  name: installedProducts
  type: array
- description: Security compliance status based on assigned policies
  name: complianceStatus
  type: string
- description: Current virus definition (DAT) version
  name: datVersion
  type: string
- description: Current scan engine version
  name: engineVersion
  type: string
- description: Timestamp of the last completed full system scan
  name: lastFullScan
  type: string
- description: CPU type and model
  name: cpuType
  type: string
- description: Total physical memory in megabytes
  name: totalPhysicalMemory
  type: integer
- description: Free disk space on the system drive in megabytes
  name: freeDiskSpace
  type: integer
provider_name: McAfee (Trellix)
provider_slug: mcafee
schema_file: json-schema/mcafee-endpoint-schema.json
slug: mcafee-endpoint
source_filename: mcafee-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.mcafee.com/schemas/mcafee/endpoint.json\",\n  \"title\": \"McAfee Managed Endpoint\",\n  \"description\": \"A managed endpoint (system) registered in McAfee ePO or MVISION, representing a computer, server, or device with McAfee security products installed and managed through the centralized console.\",\n  \"type\": \"object\",\n  \"required\": [\"computerName\", \"agentGuid\"],\n  \"properties\": {\n    \"agentGuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique McAfee Agent GUID identifying the endpoint\"\n    },\n    \"computerName\": {\n      \"type\": \"string\",\n      \"description\": \"NetBIOS or hostname of the endpoint\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"ipAddress\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"Primary IPv4 address of the endpoint\"\n \
  \   },\n    \"ipv6Address\": {\n      \"type\": \"string\",\n      \"format\": \"ipv6\",\n      \"description\": \"IPv6 address of the endpoint\"\n    },\n    \"macAddress\": {\n      \"type\": \"string\",\n      \"pattern\": \"^([0-9A-Fa-f]{2}:){5}[0-9A-Fa-f]{2}$\",\n      \"description\": \"MAC address of the primary network adapter\"\n    },\n    \"operatingSystem\": {\n      \"$ref\": \"#/$defs/OperatingSystem\"\n    },\n    \"domainName\": {\n      \"type\": \"string\",\n      \"description\": \"Active Directory domain or workgroup name\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"Currently logged-in user name\"\n    },\n    \"agentVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Installed McAfee Agent version\",\n      \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.\\\\d+(\\\\.\\\\d+)?$\"\n    },\n    \"agentStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"managed\", \"unmanaged\", \"inactive\"],\n      \"description\"\
  : \"Management state of the McAfee Agent\"\n    },\n    \"lastCommunication\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last agent-server communication\"\n    },\n    \"systemGroupPath\": {\n      \"type\": \"string\",\n      \"description\": \"Full path in the ePO System Tree (e.g., My Organization/Workstations/Finance)\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags applied to this endpoint in ePO\"\n    },\n    \"installedProducts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/InstalledProduct\"\n      },\n      \"description\": \"McAfee security products installed on the endpoint\"\n    },\n    \"complianceStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\"compliant\", \"non-compliant\", \"unknown\"],\n      \"description\": \"Security compliance status based on assigned policies\"\
  \n    },\n    \"datVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Current virus definition (DAT) version\"\n    },\n    \"engineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Current scan engine version\"\n    },\n    \"lastFullScan\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last completed full system scan\"\n    },\n    \"cpuType\": {\n      \"type\": \"string\",\n      \"description\": \"CPU type and model\"\n    },\n    \"totalPhysicalMemory\": {\n      \"type\": \"integer\",\n      \"description\": \"Total physical memory in megabytes\"\n    },\n    \"freeDiskSpace\": {\n      \"type\": \"integer\",\n      \"description\": \"Free disk space on the system drive in megabytes\"\n    }\n  },\n  \"$defs\": {\n    \"OperatingSystem\": {\n      \"type\": \"object\",\n      \"description\": \"Operating system information for the endpoint\",\n      \"properties\": {\n        \"platform\"\
  : {\n          \"type\": \"string\",\n          \"enum\": [\"Windows\", \"macOS\", \"Linux\"],\n          \"description\": \"Operating system platform\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system name (e.g., Windows 11 Enterprise, macOS Ventura)\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system version string\"\n        },\n        \"buildNumber\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system build number\"\n        },\n        \"architecture\": {\n          \"type\": \"string\",\n          \"enum\": [\"x86\", \"x64\", \"ARM64\"],\n          \"description\": \"System architecture\"\n        },\n        \"servicePack\": {\n          \"type\": \"string\",\n          \"description\": \"Service pack level (Windows only)\"\n        }\n      }\n    },\n    \"InstalledProduct\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A McAfee security product installed on the endpoint\",\n      \"properties\": {\n        \"productId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique product identifier\"\n        },\n        \"productName\": {\n          \"type\": \"string\",\n          \"description\": \"Product display name\"\n        },\n        \"productVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Installed product version\"\n        },\n        \"hotfixVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Applied hotfix or patch version\"\n        },\n        \"installDate\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Product installation timestamp\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mcafee/refs/heads/main/json-schema/mcafee-endpoint-schema.json
tags:
- Antivirus
- Cybersecurity
- Endpoint Protection
- Security
- Threat Intelligence
title: McAfee Managed Endpoint
---
