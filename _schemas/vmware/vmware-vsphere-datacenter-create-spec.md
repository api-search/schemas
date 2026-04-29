---
description: Specification for creating a datacenter
layout: schema
name: DatacenterCreateSpec
properties_list:
- description: Name for the new datacenter
  name: name
  type: string
- description: Parent folder identifier
  name: folder
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-datacenter-create-spec-schema.json
slug: vmware-vsphere-datacenter-create-spec
source_filename: vmware-vsphere-datacenter-create-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatacenterCreateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for creating a datacenter\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new datacenter\"\n    },\n    \"folder\": {\n      \"type\": \"string\",\n      \"description\": \"Parent folder identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-datacenter-create-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: DatacenterCreateSpec
---
