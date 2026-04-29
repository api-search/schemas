---
description: Contains details of a domain.
layout: schema
name: DomainDetail
properties_list:
- description: ''
  name: domainInfo
  type: object
- description: ''
  name: configuration
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-domaindetail-schema.json
slug: amazon-swf-domaindetail
source_filename: amazon-swf-domaindetail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"domainInfo\",\n    \"configuration\"\n  ],\n  \"properties\": {\n    \"domainInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainInfo\"\n        },\n        {\n          \"description\": \"The basic information about a domain, such as its name, status, and description.\"\n        }\n      ]\n    },\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainConfiguration\"\n        },\n        {\n          \"description\": \"The domain configuration. Currently, this includes only the domain's retention period.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains details of a domain.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DomainDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-domaindetail-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DomainDetail
---
