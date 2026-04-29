---
description: Request to check coverage appetite
layout: schema
name: AppetiteRequest
properties_list:
- description: US state abbreviation
  name: state
  type: string
- description: NCCI or state class code for the business
  name: class_code
  type: string
- description: Insurance product type
  name: product_type
  type: string
- description: Annual payroll amount
  name: payroll
  type: number
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
schema_file: json-schema/amtrust-financial-services-appetite-request-schema.json
slug: amtrust-financial-services-appetite-request
source_filename: amtrust-financial-services-appetite-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-appetite-request-schema.json\",\n  \"title\": \"AppetiteRequest\",\n  \"description\": \"Request to check coverage appetite\",\n  \"type\": \"object\",\n  \"required\": [\n    \"state\",\n    \"class_code\",\n    \"product_type\"\n  ],\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"US state abbreviation\",\n      \"example\": \"CA\"\n    },\n    \"class_code\": {\n      \"type\": \"string\",\n      \"description\": \"NCCI or state class code for the business\",\n      \"example\": \"8810\"\n    },\n    \"product_type\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance product type\",\n      \"enum\": [\n        \"workers_compensation\",\n        \"bop\",\n        \"general_liability\",\n        \"commercial_package\"\
  \n      ],\n      \"example\": \"workers_compensation\"\n    },\n    \"payroll\": {\n      \"type\": \"number\",\n      \"description\": \"Annual payroll amount\",\n      \"example\": 500000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-appetite-request-schema.json
tags:
- Commercial Insurance
- Insurance
- Property And Casualty
- Small Business
- Workers Compensation
title: AppetiteRequest
---
