---
description: A cost allocation record tracking technology spending in Apptio
layout: schema
name: CostAllocation
properties_list:
- description: Unique cost allocation identifier
  name: allocationId
  type: string
- description: Cost center or department receiving the allocation
  name: costCenter
  type: string
- description: Technology cost category (infrastructure, software, labor, etc.)
  name: category
  type: string
- description: Reporting period (YYYY-MM)
  name: period
  type: string
- description: Allocated cost amount in USD
  name: amount
  type: number
- description: Currency code
  name: currency
  type: string
- description: Technology vendor or provider
  name: vendor
  type: string
- description: Custom metadata tags for the allocation
  name: tags
  type: object
provider_name: Apptio
provider_slug: apptio
schema_file: json-schema/cost-allocation-schema.json
slug: cost-allocation
source_filename: cost-allocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apptio/main/json-schema/cost-allocation-schema.json\",\n  \"title\": \"CostAllocation\",\n  \"description\": \"A cost allocation record tracking technology spending in Apptio\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allocationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique cost allocation identifier\"\n    },\n    \"costCenter\": {\n      \"type\": \"string\",\n      \"description\": \"Cost center or department receiving the allocation\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Technology cost category (infrastructure, software, labor, etc.)\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"Reporting period (YYYY-MM)\"\n    },\n    \"amount\": {\n      \"type\": \"number\",\n      \"description\": \"Allocated cost amount in USD\"\n \
  \   },\n    \"currency\": {\n      \"type\": \"string\",\n      \"default\": \"USD\",\n      \"description\": \"Currency code\"\n    },\n    \"vendor\": {\n      \"type\": \"string\",\n      \"description\": \"Technology vendor or provider\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata tags for the allocation\"\n    }\n  },\n  \"required\": [\n    \"allocationId\",\n    \"costCenter\",\n    \"period\",\n    \"amount\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apptio/refs/heads/main/json-schema/cost-allocation-schema.json
tags:
- Analytics
- Cost Management
- IT Finance
- Technology Business Management
title: CostAllocation
---
