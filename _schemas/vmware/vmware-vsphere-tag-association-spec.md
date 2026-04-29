---
description: Specification for attaching a tag to an object
layout: schema
name: TagAssociationSpec
properties_list:
- description: Identifier of the tag to attach
  name: tag_id
  type: string
- description: Managed object reference
  name: object_id
  type: object
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-tag-association-spec-schema.json
slug: vmware-vsphere-tag-association-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagAssociationSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for attaching a tag to an object\",\n  \"properties\": {\n    \"tag_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the tag to attach\"\n    },\n    \"object_id\": {\n      \"type\": \"object\",\n      \"description\": \"Managed object reference\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-tag-association-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: TagAssociationSpec
---
