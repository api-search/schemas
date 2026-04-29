---
description: ''
layout: schema
name: Rule
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: Priority
  type: integer
- description: ''
  name: Action
  type: object
- description: ''
  name: VisibilityConfig
  type: object
provider_name: Amazon WAF
provider_slug: amazon-waf
schema_file: json-schema/amazon-waf-rule-schema.json
slug: amazon-waf-rule
source_filename: amazon-waf-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Priority\": {\n      \"type\": \"integer\"\n    },\n    \"Action\": {\n      \"type\": \"object\"\n    },\n    \"VisibilityConfig\": {\n      \"$ref\": \"#/components/schemas/VisibilityConfig\"\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Priority\",\n    \"VisibilityConfig\"\n  ],\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Rule\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-waf/refs/heads/main/json-schema/amazon-waf-rule-schema.json
tags:
- AWS
- Bot Management
- Ddos Protection
- Security
- WAF
- Web Application Firewall
title: Rule
---
