---
description: ''
layout: schema
name: PropertyDifference
properties_list:
- description: ''
  name: PropertyPath
  type: string
- description: ''
  name: ExpectedValue
  type: string
- description: ''
  name: ActualValue
  type: string
- description: ''
  name: DifferenceType
  type: string
provider_name: AWS CloudFormation
provider_slug: cloudformation
schema_file: json-schema/cloudformation-property-difference-schema.json
slug: cloudformation-property-difference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PropertyDifference\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PropertyPath\": {\n      \"type\": \"string\"\n    },\n    \"ExpectedValue\": {\n      \"type\": \"string\"\n    },\n    \"ActualValue\": {\n      \"type\": \"string\"\n    },\n    \"DifferenceType\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudformation/refs/heads/main/json-schema/cloudformation-property-difference-schema.json
tags:
- Automation
- AWS
- Cloud Resources
- IaC
- Infrastructure As Code
- Stack Management
title: PropertyDifference
---
