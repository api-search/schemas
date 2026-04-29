---
description: ''
layout: schema
name: DeprecateDomainInput
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-deprecatedomaininput-schema.json
slug: amazon-swf-deprecatedomaininput
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"title\": \"DeprecateDomainInput\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain to deprecate.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-deprecatedomaininput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DeprecateDomainInput
---
