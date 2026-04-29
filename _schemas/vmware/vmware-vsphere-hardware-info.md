---
description: Virtual hardware configuration
layout: schema
name: HardwareInfo
properties_list:
- description: Virtual hardware version (e.g., VMX_21)
  name: version
  type: string
- description: Hardware upgrade policy
  name: upgrade_policy
  type: string
- description: Target hardware version for upgrade
  name: upgrade_version
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-hardware-info-schema.json
slug: vmware-vsphere-hardware-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HardwareInfo\",\n  \"type\": \"object\",\n  \"description\": \"Virtual hardware configuration\",\n  \"properties\": {\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual hardware version (e.g., VMX_21)\"\n    },\n    \"upgrade_policy\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware upgrade policy\"\n    },\n    \"upgrade_version\": {\n      \"type\": \"string\",\n      \"description\": \"Target hardware version for upgrade\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-hardware-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: HardwareInfo
---
