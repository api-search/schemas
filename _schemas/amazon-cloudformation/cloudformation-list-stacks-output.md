---
description: ListStacksOutput schema
layout: schema
name: ListStacksOutput
properties_list:
- description: ''
  name: StackSummaries
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-list-stacks-output-schema.json
slug: cloudformation-list-stacks-output
source_filename: cloudformation-list-stacks-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-list-stacks-output-schema.json\",\n  \"title\": \"ListStacksOutput\",\n  \"description\": \"ListStacksOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StackSummaries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"StackId\": {\n            \"type\": \"string\"\n          },\n          \"StackName\": {\n            \"type\": \"string\"\n          },\n          \"StackStatus\": {\n            \"type\": \"string\"\n          },\n          \"CreationTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"DeletionTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"LastUpdatedTime\"\
  : {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"TemplateDescription\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-list-stacks-output-schema.json
tags:
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: ListStacksOutput
---
