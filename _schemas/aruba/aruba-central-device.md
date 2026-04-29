---
description: Represents a device in the Aruba Central inventory including access points, switches, gateways, and SD-WAN appliances.
layout: schema
name: Device
properties_list:
- description: Unique serial number of the device.
  name: serial
  type: string
- description: MAC address of the device.
  name: macaddr
  type: string
- description: Type classification of the device.
  name: device_type
  type: string
- description: Hardware model name.
  name: model
  type: string
- description: Current firmware version running on the device.
  name: firmware_version
  type: string
- description: Current operational status.
  name: status
  type: string
- description: Name of the configuration group the device belongs to.
  name: group_name
  type: string
- description: Name of the site the device is assigned to.
  name: site
  type: string
- description: IP address of the device.
  name: ip_address
  type: string
- description: Labels assigned to the device.
  name: labels
  type: array
- description: Aruba part number for the device hardware.
  name: aruba_part_no
  type: string
- description: Customer ID associated with the device.
  name: customer_id
  type: string
- description: Customer name associated with the device.
  name: customer_name
  type: string
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-device-schema.json
slug: aruba-central-device
source_filename: aruba-central-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Device\",\n  \"type\": \"object\",\n  \"description\": \"Represents a device in the Aruba Central inventory including access points, switches, gateways, and SD-WAN appliances.\",\n  \"properties\": {\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Unique serial number of the device.\"\n    },\n    \"macaddr\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address of the device.\"\n    },\n    \"device_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type classification of the device.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware model name.\"\n    },\n    \"firmware_version\": {\n      \"type\": \"string\",\n      \"description\": \"Current firmware version running on the device.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status.\"\
  \n    },\n    \"group_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the configuration group the device belongs to.\"\n    },\n    \"site\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the site the device is assigned to.\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the device.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"description\": \"Labels assigned to the device.\"\n    },\n    \"aruba_part_no\": {\n      \"type\": \"string\",\n      \"description\": \"Aruba part number for the device hardware.\"\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"Customer ID associated with the device.\"\n    },\n    \"customer_name\": {\n      \"type\": \"string\",\n      \"description\": \"Customer name associated with the device.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-device-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: Device
---
