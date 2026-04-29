---
description: Specification for creating a tag category
layout: schema
name: TagCategoryCreateSpec
properties_list:
- description: Name for the new category
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: Cardinality of the category
  name: cardinality
  type: string
- description: Object types that can be tagged with tags in this category
  name: associable_types
  type: array
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-tag-category-create-spec-schema.json
slug: vmware-vsphere-tag-category-create-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TagCategoryCreateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for creating a tag category\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name for the new category\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"cardinality\": {\n      \"type\": \"string\",\n      \"description\": \"Cardinality of the category\"\n    },\n    \"associable_types\": {\n      \"type\": \"array\",\n      \"description\": \"Object types that can be tagged with tags in this category\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-tag-category-create-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: TagCategoryCreateSpec
---
