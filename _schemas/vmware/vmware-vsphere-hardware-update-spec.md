---
description: Specification for updating virtual hardware
layout: schema
name: HardwareUpdateSpec
properties_list:
- description: ''
  name: upgrade_policy
  type: string
- description: ''
  name: upgrade_version
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-hardware-update-spec-schema.json
slug: vmware-vsphere-hardware-update-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HardwareUpdateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for updating virtual hardware\",\n  \"properties\": {\n    \"upgrade_policy\": {\n      \"type\": \"string\"\n    },\n    \"upgrade_version\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-hardware-update-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: HardwareUpdateSpec
---
