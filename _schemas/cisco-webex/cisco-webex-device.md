---
description: Represents a Webex device or room system, including its configuration, connection status, and workspace assignment.
layout: schema
name: Cisco Webex Device
properties_list:
- description: Unique identifier for the device.
  name: id
  type: string
- description: Display name of the device.
  name: displayName
  type: string
- description: Workspace ID the device is assigned to.
  name: workspaceId
  type: string
- description: Person ID the device is assigned to.
  name: personId
  type: string
- description: Organization ID the device belongs to.
  name: orgId
  type: string
- description: List of device capabilities.
  name: capabilities
  type: array
- description: List of device permissions.
  name: permissions
  type: array
- description: Current connection status of the device.
  name: connectionStatus
  type: string
- description: Product name of the device.
  name: product
  type: string
- description: Device type.
  name: type
  type: string
- description: Tags assigned to the device.
  name: tags
  type: array
- description: IP address of the device.
  name: ip
  type: string
- description: MAC address of the device.
  name: mac
  type: string
- description: Serial number of the device.
  name: serial
  type: string
- description: Software version running on the device.
  name: software
  type: string
- description: Upgrade channel for the device.
  name: upgradeChannel
  type: string
- description: Primary SIP URL of the device.
  name: primarySipUrl
  type: string
- description: SIP URLs assigned to the device.
  name: sipUrls
  type: array
- description: Error codes reported by the device.
  name: errorCodes
  type: array
- description: Date and time the device was created.
  name: created
  type: string
- description: Date and time the device was first seen.
  name: firstSeen
  type: string
- description: Date and time the device was last seen.
  name: lastSeen
  type: string
provider_name: Cisco Webex
provider_slug: cisco-webex
schema_file: json-schema/cisco-webex-device-schema.json
slug: cisco-webex-device
source_filename: cisco-webex-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.webex.com/schemas/device.json\",\n  \"title\": \"Cisco Webex Device\",\n  \"description\": \"Represents a Webex device or room system, including its configuration, connection status, and workspace assignment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the device.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the device.\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"Workspace ID the device is assigned to.\"\n    },\n    \"personId\": {\n      \"type\": \"string\",\n      \"description\": \"Person ID the device is assigned to.\"\n    },\n    \"orgId\": {\n      \"type\": \"string\",\n      \"description\": \"Organization ID the device belongs to.\"\n    },\n    \"capabilities\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"List of device capabilities.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"permissions\": {\n      \"type\": \"array\",\n      \"description\": \"List of device permissions.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"connectionStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Current connection status of the device.\",\n      \"enum\": [\"connected\", \"disconnected\", \"connected_with_issues\"]\n    },\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"Product name of the device.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Device type.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the device.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"IP address\
  \ of the device.\"\n    },\n    \"mac\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address of the device.\"\n    },\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the device.\"\n    },\n    \"software\": {\n      \"type\": \"string\",\n      \"description\": \"Software version running on the device.\"\n    },\n    \"upgradeChannel\": {\n      \"type\": \"string\",\n      \"description\": \"Upgrade channel for the device.\"\n    },\n    \"primarySipUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Primary SIP URL of the device.\"\n    },\n    \"sipUrls\": {\n      \"type\": \"array\",\n      \"description\": \"SIP URLs assigned to the device.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"errorCodes\": {\n      \"type\": \"array\",\n      \"description\": \"Error codes reported by the device.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"created\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the device was created.\"\n    },\n    \"firstSeen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the device was first seen.\"\n    },\n    \"lastSeen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the device was last seen.\"\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-webex/refs/heads/main/json-schema/cisco-webex-device-schema.json
tags:
- Collaboration
- Communications
- Meetings
- Messaging
- Teams
- Video Conferencing
title: Cisco Webex Device
---
