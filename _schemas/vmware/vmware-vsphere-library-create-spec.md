---
description: Specification for creating a content library
layout: schema
name: LibraryCreateSpec
properties_list:
- description: Name for the new content library
  name: name
  type: string
- description: Description of the content library
  name: description
  type: string
- description: Library type
  name: type
  type: string
- description: Storage backings for the library content
  name: storage_backings
  type: array
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-library-create-spec-schema.json
slug: vmware-vsphere-library-create-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibraryCreateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for creating a content library\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new content library\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the content library\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Library type\"\n    },\n    \"storage_backings\": {\n      \"type\": \"array\",\n      \"description\": \"Storage backings for the library content\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-library-create-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: LibraryCreateSpec
---
