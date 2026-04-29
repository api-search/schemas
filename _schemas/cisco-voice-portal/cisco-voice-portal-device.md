---
description: Schema for a CVP managed device. Devices are the server components that make up a CVP deployment, including Call Servers, VXML Servers, Reporting Servers, and Media Servers. Devices are registered with and managed through the CVP OAMP Server.
layout: schema
name: Cisco Voice Portal Device
properties_list:
- description: Unique identifier for the device assigned by the OAMP Server
  name: deviceId
  type: string
- description: Fully qualified hostname of the device
  name: hostname
  type: string
- description: IPv4 address of the device
  name: ipAddress
  type: string
- description: Type of CVP server component
  name: deviceType
  type: string
- description: Administrator-defined description of the device
  name: description
  type: string
- description: Current operational status
  name: status
  type: string
- description: Installed CVP software version
  name: version
  type: string
- description: Timestamp of the last successful communication with the device
  name: lastContact
  type: string
- description: Services running on the device
  name: services
  type: array
- description: ''
  name: resourceUtilization
  type: object
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-device.json
slug: cisco-voice-portal-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-voice-portal/json-schema/cisco-voice-portal-device.json\",\n  \"title\": \"Cisco Voice Portal Device\",\n  \"description\": \"Schema for a CVP managed device. Devices are the server components that make up a CVP deployment, including Call Servers, VXML Servers, Reporting Servers, and Media Servers. Devices are registered with and managed through the CVP OAMP Server.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the device assigned by the OAMP Server\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified hostname of the device\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"IPv4 address of the device\"\n    },\n    \"deviceType\": {\n      \"type\"\
  : \"string\",\n      \"enum\": [\"CallServer\", \"VXMLServer\", \"ReportingServer\", \"MediaServer\", \"OAMPServer\"],\n      \"description\": \"Type of CVP server component\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Administrator-defined description of the device\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"online\", \"offline\", \"maintenance\", \"error\"],\n      \"description\": \"Current operational status\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Installed CVP software version\"\n    },\n    \"lastContact\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last successful communication with the device\"\n    },\n    \"services\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DeviceService\"\n      },\n      \"description\": \"Services running on the device\"\n    },\n \
  \   \"resourceUtilization\": {\n      \"$ref\": \"#/$defs/ResourceUtilization\"\n    }\n  },\n  \"required\": [\"deviceId\", \"hostname\", \"ipAddress\", \"deviceType\"],\n  \"$defs\": {\n    \"DeviceService\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Service name\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"running\", \"stopped\", \"error\"],\n          \"description\": \"Service operational status\"\n        },\n        \"uptime\": {\n          \"type\": \"string\",\n          \"description\": \"Service uptime duration\"\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"Network port the service listens on\"\n        }\n      },\n      \"required\": [\"name\", \"status\"]\n    },\n    \"ResourceUtilization\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"cpuUsage\": {\n  \
  \        \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"CPU usage percentage\"\n        },\n        \"memoryUsage\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"Memory usage percentage\"\n        },\n        \"diskUsage\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"description\": \"Disk usage percentage\"\n        },\n        \"activeCalls\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of active calls on this device\"\n        },\n        \"timestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-device.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: Cisco Voice Portal Device
---
