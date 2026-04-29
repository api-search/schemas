---
description: Content library details
layout: schema
name: LibraryInfo
properties_list:
- description: Unique identifier of the content library
  name: id
  type: string
- description: Name of the content library
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: creation_time
  type: string
- description: ''
  name: last_modified_time
  type: string
- description: ''
  name: last_sync_time
  type: string
- description: ''
  name: storage_backings
  type: array
- description: ''
  name: version
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-library-info-schema.json
slug: vmware-vsphere-library-info
source_filename: vmware-vsphere-library-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibraryInfo\",\n  \"type\": \"object\",\n  \"description\": \"Content library details\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the content library\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the content library\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"creation_time\": {\n      \"type\": \"string\"\n    },\n    \"last_modified_time\": {\n      \"type\": \"string\"\n    },\n    \"last_sync_time\": {\n      \"type\": \"string\"\n    },\n    \"storage_backings\": {\n      \"type\": \"array\"\n    },\n    \"version\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-library-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: LibraryInfo
---
