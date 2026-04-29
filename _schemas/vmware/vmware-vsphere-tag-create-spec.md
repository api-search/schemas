---
description: Specification for creating a tag
layout: schema
name: TagCreateSpec
properties_list:
- description: Name for the new tag
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Identifier of the parent category
  name: category_id
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-tag-create-spec-schema.json
slug: vmware-vsphere-tag-create-spec
source_filename: vmware-vsphere-tag-create-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagCreateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for creating a tag\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new tag\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"category_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the parent category\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-tag-create-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: TagCreateSpec
---
