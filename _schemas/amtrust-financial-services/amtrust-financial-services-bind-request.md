---
description: Request to bind a quoted policy
layout: schema
name: BindRequest
properties_list:
- description: Agent electronic signature confirming bind intent
  name: agent_signature
  type: string
- description: Payment method for premium
  name: payment_method
  type: string
- description: Optional notes for the policy
  name: additional_notes
  type: string
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
schema_file: json-schema/amtrust-financial-services-bind-request-schema.json
slug: amtrust-financial-services-bind-request
source_filename: amtrust-financial-services-bind-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-bind-request-schema.json\",\n  \"title\": \"BindRequest\",\n  \"description\": \"Request to bind a quoted policy\",\n  \"type\": \"object\",\n  \"required\": [\n    \"agent_signature\"\n  ],\n  \"properties\": {\n    \"agent_signature\": {\n      \"type\": \"string\",\n      \"description\": \"Agent electronic signature confirming bind intent\",\n      \"example\": \"John Smith\"\n    },\n    \"payment_method\": {\n      \"type\": \"string\",\n      \"description\": \"Payment method for premium\",\n      \"enum\": [\n        \"direct_bill\",\n        \"agency_bill\"\n      ],\n      \"example\": \"direct_bill\"\n    },\n    \"additional_notes\": {\n      \"type\": \"string\",\n      \"description\": \"Optional notes for the policy\",\n      \"example\": \"Insured prefers\
  \ monthly installments\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/json-schema/amtrust-financial-services-bind-request-schema.json
tags:
- Commercial Insurance
- Insurance
- Property And Casualty
- Small Business
- Workers Compensation
title: BindRequest
---
