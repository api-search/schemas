---
description: ''
layout: schema
name: Chef Compliance Profile
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: summary
  type: string
- description: ''
  name: license
  type: string
- description: ''
  name: supports
  type: array
- description: ''
  name: controls
  type: array
provider_name: Chef
provider_slug: chef
schema_file: json-schema/chef-compliance-profile-schema.json
slug: chef-compliance-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.chef.io/schemas/compliance-profile.json\",\n  \"title\": \"Chef Compliance Profile\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"version\"],\n  \"properties\": {\n    \"name\": { \"type\": \"string\" },\n    \"title\": { \"type\": \"string\" },\n    \"version\": { \"type\": \"string\" },\n    \"summary\": { \"type\": \"string\" },\n    \"license\": { \"type\": \"string\" },\n    \"supports\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"object\" }\n    },\n    \"controls\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\" },\n          \"title\": { \"type\": \"string\" },\n          \"impact\": { \"type\": \"number\" }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/json-schema/chef-compliance-profile-schema.json
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
title: Chef Compliance Profile
---
