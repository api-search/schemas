---
description: Specification for creating a virtual network adapter
layout: schema
name: EthernetCreateSpec
properties_list:
- description: Adapter emulation type
  name: type
  type: string
- description: ''
  name: mac_type
  type: string
- description: MAC address (required when mac_type is MANUAL)
  name: mac_address
  type: string
- description: ''
  name: backing
  type: object
- description: ''
  name: start_connected
  type: boolean
- description: ''
  name: allow_guest_control
  type: boolean
- description: ''
  name: wake_on_lan_enabled
  type: boolean
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-ethernet-create-spec-schema.json
slug: vmware-vsphere-ethernet-create-spec
source_filename: vmware-vsphere-ethernet-create-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EthernetCreateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for creating a virtual network adapter\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Adapter emulation type\"\n    },\n    \"mac_type\": {\n      \"type\": \"string\"\n    },\n    \"mac_address\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address (required when mac_type is MANUAL)\"\n    },\n    \"backing\": {\n      \"type\": \"object\"\n    },\n    \"start_connected\": {\n      \"type\": \"boolean\"\n    },\n    \"allow_guest_control\": {\n      \"type\": \"boolean\"\n    },\n    \"wake_on_lan_enabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-ethernet-create-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: EthernetCreateSpec
---
