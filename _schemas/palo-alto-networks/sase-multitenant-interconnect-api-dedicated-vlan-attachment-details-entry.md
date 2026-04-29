---
description: DedicatedVlanAttachmentDetailsEntry schema from SP Interconnect Manage APIs
layout: schema
name: DedicatedVlanAttachmentDetailsEntry
properties_list:
- description: ''
  name: edgeAvailability
  type: string
- description: ''
  name: bandwidth
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-interconnect-api-dedicated-vlan-attachment-details-entry-schema.json
slug: sase-multitenant-interconnect-api-dedicated-vlan-attachment-details-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DedicatedVlanAttachmentDetailsEntry\",\n  \"description\": \"DedicatedVlanAttachmentDetailsEntry schema from SP Interconnect Manage APIs\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-dedicated-vlan-attachment-details-entry-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"edgeAvailability\": {\n      \"type\": \"string\"\n    },\n    \"bandwidth\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"BPS_50M\",\n        \"BPS_100M\",\n        \"BPS_200M\",\n        \"BPS_300M\",\n        \"BPS_400M\",\n        \"BPS_500M\",\n        \"BPS_1G\",\n        \"BPS_2G\",\n        \"BPS_5G\",\n        \"BPS_10G\"\n      ]\n    }\n  },\n  \"required\": [\n    \"edgeAvailability\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-dedicated-vlan-attachment-details-entry-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DedicatedVlanAttachmentDetailsEntry
---
