---
description: Schema representing a Juniper network device across management platforms including Junos Space, Mist, and Apstra. Covers routers, switches, firewalls, access points, and SD-WAN edge devices.
layout: schema
name: Juniper Network Device
properties_list:
- description: Unique identifier for the device
  name: id
  type: string
- description: Device hostname or display name
  name: name
  type: string
- description: Device serial number
  name: serial_number
  type: string
- description: MAC address of the device
  name: mac_address
  type: string
- description: Device hardware model (e.g., SRX340, QFX5120, AP43, MX204)
  name: model
  type: string
- description: Juniper device product family
  name: device_family
  type: string
- description: Functional type of the device
  name: device_type
  type: string
- description: Operating system version (Junos, Mist firmware, etc.)
  name: os_version
  type: string
- description: Management IP address
  name: management_ip
  type: string
- description: Current operational status
  name: status
  type: string
- description: Device uptime in seconds
  name: uptime
  type: integer
- description: Physical location of the device
  name: location
  type: object
- description: Network interfaces on the device
  name: interfaces
  type: array
- description: Device configuration metadata
  name: configuration
  type: object
- description: Tags or labels associated with the device
  name: tags
  type: array
- description: Organization identifier
  name: org_id
  type: string
- description: Timestamp when the device was registered
  name: created_at
  type: string
- description: Timestamp of last update
  name: updated_at
  type: string
provider_name: Juniper Networks
provider_slug: juniper
schema_file: json-schema/juniper-network-device.json
slug: juniper-network-device
source_filename: juniper-network-device.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/juniper/json-schema/juniper-network-device.json\",\n  \"title\": \"Juniper Network Device\",\n  \"description\": \"Schema representing a Juniper network device across management platforms including Junos Space, Mist, and Apstra. Covers routers, switches, firewalls, access points, and SD-WAN edge devices.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the device\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Device hostname or display name\"\n    },\n    \"serial_number\": {\n      \"type\": \"string\",\n      \"description\": \"Device serial number\"\n    },\n    \"mac_address\": {\n      \"type\": \"string\",\n      \"pattern\": \"^([0-9A-Fa-f]{2}:){5}[0-9A-Fa-f]{2}$\",\n      \"description\": \"MAC address of the device\"\n    },\n   \
  \ \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Device hardware model (e.g., SRX340, QFX5120, AP43, MX204)\"\n    },\n    \"device_family\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SRX\",\n        \"MX\",\n        \"EX\",\n        \"QFX\",\n        \"PTX\",\n        \"ACX\",\n        \"NFX\",\n        \"AP\",\n        \"SSR\"\n      ],\n      \"description\": \"Juniper device product family\"\n    },\n    \"device_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"router\",\n        \"switch\",\n        \"firewall\",\n        \"access_point\",\n        \"gateway\",\n        \"wan_edge\"\n      ],\n      \"description\": \"Functional type of the device\"\n    },\n    \"os_version\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system version (Junos, Mist firmware, etc.)\"\n    },\n    \"management_ip\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"Management IP address\"\
  \n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"connected\",\n        \"disconnected\",\n        \"upgrading\",\n        \"restarting\",\n        \"provisioning\",\n        \"error\"\n      ],\n      \"description\": \"Current operational status\"\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Device uptime in seconds\"\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"Physical location of the device\",\n      \"properties\": {\n        \"site_id\": {\n          \"type\": \"string\",\n          \"description\": \"Site or facility identifier\"\n        },\n        \"site_name\": {\n          \"type\": \"string\",\n          \"description\": \"Site or facility name\"\n        },\n        \"address\": {\n          \"type\": \"string\",\n          \"description\": \"Physical address\"\n        },\n        \"latitude\": {\n          \"type\": \"number\",\n    \
  \      \"minimum\": -90,\n          \"maximum\": 90\n        },\n        \"longitude\": {\n          \"type\": \"number\",\n          \"minimum\": -180,\n          \"maximum\": 180\n        },\n        \"floor\": {\n          \"type\": \"string\",\n          \"description\": \"Building floor\"\n        },\n        \"rack\": {\n          \"type\": \"string\",\n          \"description\": \"Rack identifier\"\n        }\n      }\n    },\n    \"interfaces\": {\n      \"type\": \"array\",\n      \"description\": \"Network interfaces on the device\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Interface name (e.g., ge-0/0/0, xe-0/0/1)\"\n          },\n          \"admin_status\": {\n            \"type\": \"string\",\n            \"enum\": [\"up\", \"down\"]\n          },\n          \"oper_status\": {\n            \"type\": \"string\",\n            \"enum\": [\"up\", \"down\"\
  ]\n          },\n          \"speed\": {\n            \"type\": \"string\",\n            \"description\": \"Interface speed (e.g., 1G, 10G, 25G, 40G, 100G)\"\n          },\n          \"mtu\": {\n            \"type\": \"integer\",\n            \"description\": \"Maximum Transmission Unit\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"ip_addresses\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\",\n              \"description\": \"IP address in CIDR notation\"\n            }\n          },\n          \"mac_address\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"configuration\": {\n      \"type\": \"object\",\n      \"description\": \"Device configuration metadata\",\n      \"properties\": {\n        \"last_committed\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"last_committed_by\": {\n     \
  \     \"type\": \"string\"\n        },\n        \"sync_status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"in_sync\",\n            \"out_of_sync\",\n            \"unknown\"\n          ]\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags or labels associated with the device\"\n    },\n    \"org_id\": {\n      \"type\": \"string\",\n      \"description\": \"Organization identifier\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the device was registered\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of last update\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"device_type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper/refs/heads/main/json-schema/juniper-network-device.json
tags:
- AI
- Automation
- Cloud
- Enterprise
- Networking
- SDN
- Security
title: Juniper Network Device
---
