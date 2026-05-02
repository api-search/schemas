---
description: Schema for a Juniper Mist managed device. Devices include Mist-managed access points (AP12, AP32, AP33, AP34, AP43, AP45, AP63, AP64), EX-series switches (EX2300, EX3400, EX4100, EX4300, EX4400, EX4650), and SRX/SSR gateways (SRX300, SRX320, SRX340, SRX345, SRX1500, SSR120, SSR130). Each device is claimed to an organization, optionally assigned to a site, and managed through the Mist cloud. Devices receive configuration from the cloud, report telemetry, and can be placed on floor plan maps for location-aware management.
layout: schema
name: Juniper Mist Device
properties_list:
- description: Device unique identifier assigned by the Mist cloud upon claiming.
  name: id
  type: string
- description: Organization identifier the device is claimed to.
  name: org_id
  type: string
- description: Site identifier the device is assigned to. Null if the device is in the organization inventory but not assigned to a site.
  name: site_id
  type:
  - string
  - 'null'
- description: Device display name. Defaults to the device model and MAC address if not set.
  name: name
  type: string
- description: Device type. 'ap' for wireless access points, 'switch' for EX-series wired switches, 'gateway' for SRX/SSR WAN gateways.
  name: type
  type: string
- description: 'Hardware model identifier. Examples: AP45, AP63, EX4100-48P, EX4400-24T, SRX320, SSR130.'
  name: model
  type: string
- description: Hardware serial number printed on the device chassis. Used for device claiming via claim code or serial number.
  name: serial
  type: string
- description: Device primary MAC address in colon-separated format (e.g., 5c:5b:35:aa:bb:cc). Serves as the device unique hardware identifier.
  name: mac
  type: string
- description: Device management IP address. Assigned via DHCP or static configuration.
  name: ip
  type: string
- description: Current firmware version running on the device. Mist manages firmware upgrades through the cloud.
  name: version
  type: string
- description: Hardware revision identifier.
  name: hw_rev
  type: string
- description: Floor plan map ID where the device is placed. Used for indoor location and RF planning visualization.
  name: map_id
  type:
  - string
  - 'null'
- description: X coordinate position on the floor plan map in pixels.
  name: x
  type: number
- description: Y coordinate position on the floor plan map in pixels.
  name: y
  type: number
- description: AP mounting orientation in degrees (0-359) relative to the map north direction. Affects directional antenna patterns and location calculation accuracy.
  name: orientation
  type: integer
- description: AP mounting height above floor level in meters. Used for 3D location calculation and RF propagation modeling.
  name: height
  type: number
- description: Free-form notes for operational documentation.
  name: notes
  type: string
- description: Device creation timestamp in epoch seconds.
  name: created_time
  type: number
- description: Last modification timestamp in epoch seconds.
  name: modified_time
  type: number
provider_name: Juniper Networks
provider_slug: juniper-networks
schema_file: json-schema/juniper-networks-mist-device-schema.json
slug: juniper-networks-mist-device
source_filename: juniper-networks-mist-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-mist-device-schema.json\",\n  \"title\": \"Juniper Mist Device\",\n  \"description\": \"Schema for a Juniper Mist managed device. Devices include Mist-managed access points (AP12, AP32, AP33, AP34, AP43, AP45, AP63, AP64), EX-series switches (EX2300, EX3400, EX4100, EX4300, EX4400, EX4650), and SRX/SSR gateways (SRX300, SRX320, SRX340, SRX345, SRX1500, SSR120, SSR130). Each device is claimed to an organization, optionally assigned to a site, and managed through the Mist cloud. Devices receive configuration from the cloud, report telemetry, and can be placed on floor plan maps for location-aware management.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Device unique identifier assigned\
  \ by the Mist cloud upon claiming.\"\n    },\n    \"org_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Organization identifier the device is claimed to.\"\n    },\n    \"site_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uuid\",\n      \"description\": \"Site identifier the device is assigned to. Null if the device is in the organization inventory but not assigned to a site.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Device display name. Defaults to the device model and MAC address if not set.\",\n      \"maxLength\": 64\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"ap\", \"switch\", \"gateway\"],\n      \"description\": \"Device type. 'ap' for wireless access points, 'switch' for EX-series wired switches, 'gateway' for SRX/SSR WAN gateways.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware model identifier. Examples:\
  \ AP45, AP63, EX4100-48P, EX4400-24T, SRX320, SSR130.\"\n    },\n    \"serial\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware serial number printed on the device chassis. Used for device claiming via claim code or serial number.\"\n    },\n    \"mac\": {\n      \"type\": \"string\",\n      \"description\": \"Device primary MAC address in colon-separated format (e.g., 5c:5b:35:aa:bb:cc). Serves as the device unique hardware identifier.\",\n      \"pattern\": \"^[0-9a-f]{2}(:[0-9a-f]{2}){5}$\"\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"description\": \"Device management IP address. Assigned via DHCP or static configuration.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Current firmware version running on the device. Mist manages firmware upgrades through the cloud.\"\n    },\n    \"hw_rev\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware revision identifier.\"\n    },\n    \"map_id\": {\n   \
  \   \"type\": [\"string\", \"null\"],\n      \"format\": \"uuid\",\n      \"description\": \"Floor plan map ID where the device is placed. Used for indoor location and RF planning visualization.\"\n    },\n    \"x\": {\n      \"type\": \"number\",\n      \"description\": \"X coordinate position on the floor plan map in pixels.\"\n    },\n    \"y\": {\n      \"type\": \"number\",\n      \"description\": \"Y coordinate position on the floor plan map in pixels.\"\n    },\n    \"orientation\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 359,\n      \"description\": \"AP mounting orientation in degrees (0-359) relative to the map north direction. Affects directional antenna patterns and location calculation accuracy.\"\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"AP mounting height above floor level in meters. Used for 3D location calculation and RF propagation modeling.\"\n    },\n    \"notes\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Free-form notes for operational documentation.\"\n    },\n    \"created_time\": {\n      \"type\": \"number\",\n      \"description\": \"Device creation timestamp in epoch seconds.\"\n    },\n    \"modified_time\": {\n      \"type\": \"number\",\n      \"description\": \"Last modification timestamp in epoch seconds.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/juniper-networks/refs/heads/main/json-schema/juniper-networks-mist-device-schema.json
tags:
- Automation
- Cloud
- Data Center
- Enterprise
- Networking
- SDN
- Security
title: Juniper Mist Device
---
