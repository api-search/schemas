---
description: Change schema
layout: schema
name: Change
properties_list:
- description: ''
  name: Type
  type: string
- description: ''
  name: ResourceChange
  type: object
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-change-schema.json
slug: cloudformation-change
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-change-schema.json\",\n  \"title\": \"Change\",\n  \"description\": \"Change schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Resource\"\n      ]\n    },\n    \"ResourceChange\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Action\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Add\",\n            \"Modify\",\n            \"Remove\",\n            \"Import\",\n            \"Dynamic\"\n          ]\n        },\n        \"LogicalResourceId\": {\n          \"type\": \"string\"\n        },\n        \"PhysicalResourceId\": {\n          \"type\": \"string\"\n        },\n        \"ResourceType\": {\n          \"type\": \"string\"\n        },\n        \"Replacement\"\
  : {\n          \"type\": \"string\",\n          \"enum\": [\n            \"True\",\n            \"False\",\n            \"Conditional\"\n          ]\n        },\n        \"Scope\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-change-schema.json
tags:
- AWS
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: Change
---
