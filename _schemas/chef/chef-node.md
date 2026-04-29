---
description: ''
layout: schema
name: Chef Node
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: chef_environment
  type: string
- description: ''
  name: run_list
  type: array
- description: ''
  name: automatic
  type: object
- description: ''
  name: default
  type: object
- description: ''
  name: normal
  type: object
- description: ''
  name: override
  type: object
provider_name: Chef
provider_slug: chef
schema_file: json-schema/chef-node-schema.json
slug: chef-node
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.chef.io/schemas/node.json\",\n  \"title\": \"Chef Node\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": { \"type\": \"string\" },\n    \"chef_environment\": { \"type\": \"string\" },\n    \"run_list\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"automatic\": { \"type\": \"object\" },\n    \"default\": { \"type\": \"object\" },\n    \"normal\": { \"type\": \"object\" },\n    \"override\": { \"type\": \"object\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/json-schema/chef-node-schema.json
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
title: Chef Node
---
