---
description: ''
layout: schema
name: DescribeDomainInput
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-describedomaininput-schema.json
slug: amazon-swf-describedomaininput
source_filename: amazon-swf-describedomaininput-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"title\": \"DescribeDomainInput\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of the domain to describe.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-describedomaininput-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DescribeDomainInput
---
