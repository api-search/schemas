---
description: Specification for creating a virtual disk
layout: schema
name: DiskCreateSpec
properties_list:
- description: Host bus adapter type
  name: type
  type: string
- description: Specification for a new VMDK file
  name: new_vmdk
  type: object
- description: Existing disk backing
  name: backing
  type: object
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-disk-create-spec-schema.json
slug: vmware-vsphere-disk-create-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DiskCreateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for creating a virtual disk\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Host bus adapter type\"\n    },\n    \"new_vmdk\": {\n      \"type\": \"object\",\n      \"description\": \"Specification for a new VMDK file\"\n    },\n    \"backing\": {\n      \"type\": \"object\",\n      \"description\": \"Existing disk backing\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-disk-create-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: DiskCreateSpec
---
