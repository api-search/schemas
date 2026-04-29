---
description: Provisioned concurrency configuration for a function
layout: schema
name: ProvisionedConcurrencyConfig
properties_list:
- description: The amount of provisioned concurrency requested
  name: RequestedProvisionedConcurrentExecutions
  type: integer
- description: The amount of provisioned concurrency available
  name: AvailableProvisionedConcurrentExecutions
  type: integer
- description: The amount of provisioned concurrency allocated
  name: AllocatedProvisionedConcurrentExecutions
  type: integer
- description: The status of the allocation
  name: Status
  type: string
- description: For failed allocations, the reason the status is FAILED
  name: StatusReason
  type: string
- description: The date and time the configuration was last modified
  name: LastModified
  type: string
provider_name: AWS Lambda
provider_slug: aws-lambda
schema_file: json-schema/aws-lambda-provisioned-concurrency-config-schema.json
slug: aws-lambda-provisioned-concurrency-config
source_filename: aws-lambda-provisioned-concurrency-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProvisionedConcurrencyConfig\",\n  \"type\": \"object\",\n  \"description\": \"Provisioned concurrency configuration for a function\",\n  \"properties\": {\n    \"RequestedProvisionedConcurrentExecutions\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of provisioned concurrency requested\"\n    },\n    \"AvailableProvisionedConcurrentExecutions\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of provisioned concurrency available\"\n    },\n    \"AllocatedProvisionedConcurrentExecutions\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of provisioned concurrency allocated\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the allocation\"\n    },\n    \"StatusReason\": {\n      \"type\": \"string\",\n      \"description\": \"For failed allocations, the reason the status is FAILED\"\
  \n    },\n    \"LastModified\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the configuration was last modified\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-lambda/refs/heads/main/json-schema/aws-lambda-provisioned-concurrency-config-schema.json
tags: []
title: ProvisionedConcurrencyConfig
---
