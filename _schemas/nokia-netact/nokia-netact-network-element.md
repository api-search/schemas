---
description: A managed network element in the Nokia NetAct OSS topology (ITU-T X.700 NE)
layout: schema
name: Nokia NetAct Network Element
properties_list:
- description: X.711 Distinguished Name uniquely identifying the NE in the managed object tree
  name: distinguishedName
  type: string
- description: Managed object class (e.g., BTS, LNBTS, GNODEB, MSC, RNC, BSC)
  name: neType
  type: string
- description: Radio access or core technology generation
  name: technology
  type: string
- description: Network equipment vendor
  name: vendor
  type: string
- description: ''
  name: softwareVersion
  type: string
- description: ITU-T X.731 operational state
  name: operationalState
  type: string
- description: ITU-T X.731 administrative state
  name: administrativeState
  type: string
- description: Derived from active alarms on this NE
  name: alarmState
  type: string
- description: Management IP address
  name: ipAddress
  type: string
- description: ''
  name: location
  type: object
- description: Technology-specific managed object attribute values
  name: attributes
  type: object
provider_name: Nokia NetAct
provider_slug: nokia-netact
schema_file: json-schema/nokia-netact-network-element-schema.json
slug: nokia-netact-network-element
source_filename: nokia-netact-network-element-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/nokia-netact/refs/heads/main/json-schema/nokia-netact-network-element-schema.json\",\n  \"title\": \"Nokia NetAct Network Element\",\n  \"description\": \"A managed network element in the Nokia NetAct OSS topology (ITU-T X.700 NE)\",\n  \"type\": \"object\",\n  \"required\": [\"distinguishedName\", \"neType\"],\n  \"properties\": {\n    \"distinguishedName\": {\n      \"type\": \"string\",\n      \"description\": \"X.711 Distinguished Name uniquely identifying the NE in the managed object tree\"\n    },\n    \"neType\": {\n      \"type\": \"string\",\n      \"description\": \"Managed object class (e.g., BTS, LNBTS, GNODEB, MSC, RNC, BSC)\"\n    },\n    \"technology\": {\n      \"type\": \"string\",\n      \"enum\": [\"2G\", \"3G\", \"4G\", \"5G\", \"TRANSPORT\", \"CORE\"],\n      \"description\": \"Radio access or core technology generation\"\n\
  \    },\n    \"vendor\": {\n      \"type\": \"string\",\n      \"description\": \"Network equipment vendor\"\n    },\n    \"softwareVersion\": {\n      \"type\": \"string\"\n    },\n    \"operationalState\": {\n      \"type\": \"string\",\n      \"enum\": [\"ENABLED\", \"DISABLED\", \"UNKNOWN\"],\n      \"description\": \"ITU-T X.731 operational state\"\n    },\n    \"administrativeState\": {\n      \"type\": \"string\",\n      \"enum\": [\"LOCKED\", \"UNLOCKED\", \"SHUTTINGDOWN\"],\n      \"description\": \"ITU-T X.731 administrative state\"\n    },\n    \"alarmState\": {\n      \"type\": \"string\",\n      \"enum\": [\"CLEAR\", \"WARNING\", \"MINOR\", \"MAJOR\", \"CRITICAL\"],\n      \"description\": \"Derived from active alarms on this NE\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"Management IP address\"\n    },\n    \"location\": {\n      \"$ref\": \"#/$defs/NetworkLocation\"\n    },\n    \"attributes\": {\n \
  \     \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"Technology-specific managed object attribute values\"\n    }\n  },\n  \"$defs\": {\n    \"NetworkLocation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"latitude\": {\n          \"type\": \"number\",\n          \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        },\n        \"address\": {\n          \"type\": \"string\"\n        },\n        \"siteId\": {\n          \"type\": \"string\",\n          \"description\": \"Physical site identifier\"\n        },\n        \"siteName\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nokia-netact/refs/heads/main/json-schema/nokia-netact-network-element-schema.json
tags:
- Network Management
- OSS
- SNMP
- Telecom
title: Nokia NetAct Network Element
---
