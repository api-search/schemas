---
description: ''
layout: schema
name: Chef Role
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: run_list
  type: array
- description: ''
  name: default_attributes
  type: object
- description: ''
  name: override_attributes
  type: object
provider_name: Chef
provider_slug: chef
schema_file: json-schema/chef-role-schema.json
slug: chef-role
source_filename: chef-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.chef.io/schemas/role.json\",\n  \"title\": \"Chef Role\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": { \"type\": \"string\" },\n    \"description\": { \"type\": \"string\" },\n    \"run_list\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"default_attributes\": { \"type\": \"object\" },\n    \"override_attributes\": { \"type\": \"object\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/json-schema/chef-role-schema.json
tags:
- Application Delivery
- Automation
- Compliance
- Configuration Management
- DevOps
- DevSecOps
- Habitat
- Infrastructure as Code
- InSpec
title: Chef Role
---
