---
description: A network interface (LIF) providing data or management access
layout: schema
name: NetworkInterface
properties_list:
- description: Network interface UUID
  name: uuid
  type: string
- description: Interface name
  name: name
  type: string
- description: IP address configuration
  name: ip
  type: object
- description: Operational state of the interface
  name: state
  type: string
- description: Whether the interface is administratively enabled
  name: enabled
  type: boolean
- description: Interface scope
  name: scope
  type: string
- description: Service policy governing the interface
  name: service_policy
  type: object
- description: Current location of the interface
  name: location
  type: object
provider_name: NetApp
provider_slug: netapp
schema_file: json-schema/netapp-ontap-network-interface-schema.json
slug: netapp-ontap-network-interface
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkInterface\",\n  \"type\": \"object\",\n  \"description\": \"A network interface (LIF) providing data or management access\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Network interface UUID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Interface name\"\n    },\n    \"ip\": {\n      \"type\": \"object\",\n      \"description\": \"IP address configuration\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Operational state of the interface\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the interface is administratively enabled\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Interface scope\"\n    },\n    \"service_policy\": {\n      \"type\": \"object\",\n      \"description\": \"Service policy\
  \ governing the interface\"\n    },\n    \"location\": {\n      \"type\": \"object\",\n      \"description\": \"Current location of the interface\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/json-schema/netapp-ontap-network-interface-schema.json
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
title: NetworkInterface
---
