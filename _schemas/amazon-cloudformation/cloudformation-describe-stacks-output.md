---
description: DescribeStacksOutput schema
layout: schema
name: DescribeStacksOutput
properties_list:
- description: ''
  name: Stacks
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon CloudFormation
provider_slug: amazon-cloudformation
schema_file: json-schema/cloudformation-describe-stacks-output-schema.json
slug: cloudformation-describe-stacks-output
source_filename: cloudformation-describe-stacks-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-describe-stacks-output-schema.json\",\n  \"title\": \"DescribeStacksOutput\",\n  \"description\": \"DescribeStacksOutput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Stacks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Stack\"\n      }\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudformation/refs/heads/main/json-schema/cloudformation-describe-stacks-output-schema.json
tags:
- AWS
- CloudFormation
- Infrastructure as Code
- DevOps
- IaC
title: DescribeStacksOutput
---
