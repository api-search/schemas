---
description: Request to get datasource package history for accounts
layout: schema
name: BatchGetMembershipDatasourcesRequest
properties_list:
- description: The ARN of the behavior graph.
  name: GraphArns
  type: array
provider_name: Amazon Detective
provider_slug: amazon-detective
schema_file: json-schema/amazon-detective-batch-get-membership-datasources-request-schema.json
slug: amazon-detective-batch-get-membership-datasources-request
source_filename: amazon-detective-batch-get-membership-datasources-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-batch-get-membership-datasources-request-schema.json\",\n  \"title\": \"BatchGetMembershipDatasourcesRequest\",\n  \"description\": \"Request to get datasource package history for accounts\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GraphArns\": {\n      \"type\": \"array\",\n      \"description\": \"The ARN of the behavior graph.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"arn:aws:detective:us-east-1:123456789012:graph:abc123def456\"\n      ]\n    }\n  },\n  \"required\": [\n    \"GraphArns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-detective/refs/heads/main/json-schema/amazon-detective-batch-get-membership-datasources-request-schema.json
tags:
- Forensics
- Investigation
- Security
title: BatchGetMembershipDatasourcesRequest
---
