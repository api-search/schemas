---
description: Schema for a device managed by HPE Aruba Networking Central, covering access points, switches, gateways, and SD-WAN appliances in the device inventory.
layout: schema
name: Aruba Central Device
properties_list:
- description: Unique serial number identifying the device in the Aruba Central inventory.
  name: serial
  type: string
- description: MAC address of the device in colon-separated hexadecimal format.
  name: macaddr
  type: string
- description: Classification of the device type within the Aruba Central platform.
  name: device_type
  type: string
- description: Hardware model name or number of the device.
  name: model
  type: string
- description: Current firmware version running on the device.
  name: firmware_version
  type: string
- description: Current operational status of the device.
  name: status
  type: string
- description: IPv4 address assigned to the device.
  name: ip_address
  type: string
- description: User-configured name or hostname of the device.
  name: name
  type: string
- description: Name of the Aruba Central configuration group the device belongs to.
  name: group_name
  type: string
- description: Name of the physical site the device is assigned to.
  name: site
  type: string
- description: Labels assigned to the device for custom categorization and filtering.
  name: labels
  type: array
- description: Aruba hardware part number for the device.
  name: aruba_part_no
  type: string
- description: Aruba Central customer ID that owns the device.
  name: customer_id
  type: string
- description: Name of the customer organization that owns the device.
  name: customer_name
  type: string
- description: Deployment mode for access point devices. IAP indicates Instant AP mode, AOS10 indicates the AOS 10 architecture.
  name: ap_deployment_mode
  type: string
- description: Identifier of the Swarm or AP cluster the device belongs to (access points only).
  name: swarm_id
  type: string
- description: Name of the Swarm or AP cluster.
  name: swarm_name
  type: string
- description: Cluster identifier for the device.
  name: cluster_id
  type: string
- description: Mesh networking role of the access point.
  name: mesh_role
  type: string
- description: Number of clients currently connected to the device.
  name: client_count
  type: integer
- description: Time since last reboot in seconds.
  name: uptime
  type: integer
- description: Current CPU utilization as a percentage.
  name: cpu_utilization
  type: integer
- description: Total device memory in bytes.
  name: mem_total
  type: integer
- description: Available free memory in bytes.
  name: mem_free
  type: integer
- description: Radio interfaces on the device (access points only).
  name: radios
  type: array
- description: Physical uplink connection details.
  name: uplink
  type: object
- description: ISO 8601 timestamp of the last configuration change on the device.
  name: last_modified
  type: string
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-device-schema.json
slug: aruba-device
source_json: "{\n  \"$id\": \"https://developer.arubanetworks.com/schemas/aruba-device-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Aruba Central Device\",\n  \"description\": \"Schema for a device managed by HPE Aruba Networking Central, covering access points, switches, gateways, and SD-WAN appliances in the device inventory.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"serial\",\n    \"macaddr\",\n    \"device_type\"\n  ],\n  \"properties\": {\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Unique serial number identifying the device in the Aruba Central inventory.\",\n      \"examples\": [\n        \"CNBRJM0ABC\"\n      ]\n    },\n    \"macaddr\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address of the device in colon-separated hexadecimal format.\",\n      \"pattern\": \"^([0-9A-Fa-f]{2}:){5}[0-9A-Fa-f]{2}$\",\n      \"examples\": [\n        \"aa:bb:cc:dd:ee:ff\"\n      ]\n   \
  \ },\n    \"device_type\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the device type within the Aruba Central platform.\",\n      \"enum\": [\n        \"IAP\",\n        \"HP\",\n        \"CONTROLLER\",\n        \"GATEWAY\",\n        \"SWITCH\",\n        \"VGW\"\n      ]\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware model name or number of the device.\",\n      \"examples\": [\n        \"AP-515\",\n        \"AP-635\",\n        \"Aruba 6300M\",\n        \"Aruba 9004\"\n      ]\n    },\n    \"firmware_version\": {\n      \"type\": \"string\",\n      \"description\": \"Current firmware version running on the device.\",\n      \"examples\": [\n        \"10.4.0.0_85559\",\n        \"10.12.0001\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status of the device.\",\n      \"enum\": [\n        \"Up\",\n        \"Down\"\n      ]\n    },\n    \"ip_address\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"IPv4 address assigned to the device.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"User-configured name or hostname of the device.\",\n      \"examples\": [\n        \"AP-lobby-01\",\n        \"switch-floor2\"\n      ]\n    },\n    \"group_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Aruba Central configuration group the device belongs to.\"\n    },\n    \"site\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the physical site the device is assigned to.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels assigned to the device for custom categorization and filtering.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"aruba_part_no\": {\n      \"type\": \"string\",\n      \"description\": \"Aruba hardware part number for the device.\"\n    },\n    \"customer_id\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Aruba Central customer ID that owns the device.\"\n    },\n    \"customer_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the customer organization that owns the device.\"\n    },\n    \"ap_deployment_mode\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment mode for access point devices. IAP indicates Instant AP mode, AOS10 indicates the AOS 10 architecture.\",\n      \"enum\": [\n        \"IAP\",\n        \"AOS10\"\n      ]\n    },\n    \"swarm_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the Swarm or AP cluster the device belongs to (access points only).\"\n    },\n    \"swarm_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the Swarm or AP cluster.\"\n    },\n    \"cluster_id\": {\n      \"type\": \"string\",\n      \"description\": \"Cluster identifier for the device.\"\n    },\n    \"mesh_role\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Mesh networking role of the access point.\",\n      \"enum\": [\n        \"Portal\",\n        \"Point\",\n        \"None\"\n      ]\n    },\n    \"client_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of clients currently connected to the device.\",\n      \"minimum\": 0\n    },\n    \"uptime\": {\n      \"type\": \"integer\",\n      \"description\": \"Time since last reboot in seconds.\",\n      \"minimum\": 0\n    },\n    \"cpu_utilization\": {\n      \"type\": \"integer\",\n      \"description\": \"Current CPU utilization as a percentage.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"mem_total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total device memory in bytes.\",\n      \"minimum\": 0\n    },\n    \"mem_free\": {\n      \"type\": \"integer\",\n      \"description\": \"Available free memory in bytes.\",\n      \"minimum\": 0\n    },\n    \"radios\": {\n      \"type\": \"array\",\n      \"\
  description\": \"Radio interfaces on the device (access points only).\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Radio\"\n      }\n    },\n    \"uplink\": {\n      \"$ref\": \"#/$defs/Uplink\",\n      \"description\": \"Physical uplink connection details.\"\n    },\n    \"last_modified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp of the last configuration change on the device.\"\n    }\n  },\n  \"$defs\": {\n    \"Radio\": {\n      \"type\": \"object\",\n      \"description\": \"A radio interface on an Aruba access point, representing a physical wireless transmitter/receiver.\",\n      \"properties\": {\n        \"index\": {\n          \"type\": \"integer\",\n          \"description\": \"Radio index number (typically 0 for 2.4 GHz, 1 for 5 GHz, 2 for 6 GHz).\",\n          \"minimum\": 0\n        },\n        \"macaddr\": {\n          \"type\": \"string\",\n          \"description\": \"MAC address of the radio interface.\"\
  ,\n          \"pattern\": \"^([0-9A-Fa-f]{2}:){5}[0-9A-Fa-f]{2}$\"\n        },\n        \"band\": {\n          \"type\": \"number\",\n          \"description\": \"Operating frequency band in GHz.\",\n          \"enum\": [\n            2.4,\n            5,\n            6\n          ]\n        },\n        \"channel\": {\n          \"type\": \"string\",\n          \"description\": \"Operating channel number or channel string (e.g., '36' or '36E').\"\n        },\n        \"power\": {\n          \"type\": \"integer\",\n          \"description\": \"Configured transmit power in dBm.\"\n        },\n        \"tx_power\": {\n          \"type\": \"integer\",\n          \"description\": \"Effective transmit power in dBm after ARM adjustments.\"\n        },\n        \"utilization\": {\n          \"type\": \"integer\",\n          \"description\": \"Channel utilization percentage.\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"noise_floor\": {\n          \"type\": \"\
  integer\",\n          \"description\": \"Measured noise floor in dBm.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Operational status of the radio.\",\n          \"enum\": [\n            \"Up\",\n            \"Down\"\n          ]\n        }\n      },\n      \"required\": [\n        \"index\",\n        \"band\"\n      ]\n    },\n    \"Uplink\": {\n      \"type\": \"object\",\n      \"description\": \"Physical uplink connection details for the device.\",\n      \"properties\": {\n        \"ethernet\": {\n          \"type\": \"object\",\n          \"description\": \"Ethernet uplink properties.\",\n          \"properties\": {\n            \"port\": {\n              \"type\": \"string\",\n              \"description\": \"Ethernet port identifier.\"\n            },\n            \"speed\": {\n              \"type\": \"string\",\n              \"description\": \"Negotiated link speed (e.g., '1000Mbps').\"\n            },\n            \"duplex\"\
  : {\n              \"type\": \"string\",\n              \"description\": \"Duplex mode of the connection.\",\n              \"enum\": [\n                \"Full\",\n                \"Half\"\n              ]\n            },\n            \"poe_power\": {\n              \"type\": \"number\",\n              \"description\": \"Power over Ethernet draw in watts.\",\n              \"minimum\": 0\n            }\n          }\n        }\n      }\n    }\n  },\n  \"examples\": [\n    {\n      \"serial\": \"CNBRJM0ABC\",\n      \"macaddr\": \"aa:bb:cc:dd:ee:ff\",\n      \"device_type\": \"IAP\",\n      \"model\": \"AP-515\",\n      \"firmware_version\": \"10.4.0.0_85559\",\n      \"status\": \"Up\",\n      \"ip_address\": \"10.1.10.50\",\n      \"name\": \"AP-lobby-01\",\n      \"group_name\": \"default\",\n      \"site\": \"Headquarters\",\n      \"labels\": [\n        \"floor-1\",\n        \"lobby\"\n      ],\n      \"ap_deployment_mode\": \"AOS10\",\n      \"client_count\": 42,\n      \"uptime\"\
  : 864000,\n      \"cpu_utilization\": 15,\n      \"mem_total\": 1073741824,\n      \"mem_free\": 536870912,\n      \"radios\": [\n        {\n          \"index\": 0,\n          \"macaddr\": \"aa:bb:cc:dd:ee:f0\",\n          \"band\": 2.4,\n          \"channel\": \"6\",\n          \"power\": 18,\n          \"tx_power\": 18,\n          \"utilization\": 35,\n          \"noise_floor\": -95,\n          \"status\": \"Up\"\n        },\n        {\n          \"index\": 1,\n          \"macaddr\": \"aa:bb:cc:dd:ee:f1\",\n          \"band\": 5,\n          \"channel\": \"36\",\n          \"power\": 20,\n          \"tx_power\": 20,\n          \"utilization\": 22,\n          \"noise_floor\": -92,\n          \"status\": \"Up\"\n        }\n      ],\n      \"uplink\": {\n        \"ethernet\": {\n          \"port\": \"eth0\",\n          \"speed\": \"1000Mbps\",\n          \"duplex\": \"Full\",\n          \"poe_power\": 15.4\n        }\n      },\n      \"last_modified\": \"2026-02-28T14:30:00Z\"\n    }\n \
  \ ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-device-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: Aruba Central Device
---
