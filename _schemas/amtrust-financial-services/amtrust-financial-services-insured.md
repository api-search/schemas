---
description: Business insured information
layout: schema
name: Insured
properties_list:
- description: Legal business name
  name: name
  type: string
- description: Federal Employer Identification Number
  name: fein
  type: string
- description: NCCI or state class code
  name: class_code
  type: string
- description: ''
  name: address
  type: object
- description: Years the business has been operating
  name: years_in_business
  type: integer
- description: Total annual payroll
  name: payroll
  type: number
- description: Total number of employees
  name: employee_count
  type: integer
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
schema_file: json-schema/amtrust-financial-services-insured-schema.json
slug: amtrust-financial-services-insured
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-insured-schema.json\",\n  \"title\": \"Insured\",\n  \"description\": \"Business insured information\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"address\",\n    \"class_code\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Legal business name\",\n      \"example\": \"Acme Contracting LLC\"\n    },\n    \"fein\": {\n      \"type\": \"string\",\n      \"description\": \"Federal Employer Identification Number\",\n      \"example\": \"12-3456789\"\n    },\n    \"class_code\": {\n      \"type\": \"string\",\n      \"description\": \"NCCI or state class code\",\n      \"example\": \"8810\"\n    },\n    \"address\": {\n      \"$ref\": \"#/components/schemas/Address\"\n    },\n    \"years_in_business\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Years the business has been operating\",\n      \"example\": 5\n    },\n    \"payroll\": {\n      \"type\": \"number\",\n      \"description\": \"Total annual payroll\",\n      \"example\": 750000\n    },\n    \"employee_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of employees\",\n      \"example\": 25\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-insured-schema.json
tags:
- Commercial Insurance
- Insurance
- Property And Casualty
- Small Business
- Workers Compensation
title: Insured
---
