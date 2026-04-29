---
description: ''
layout: schema
name: Record23
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: Name
  type: string
- description: ''
  name: Pricebook2Id
  type: string
- description: ''
  name: QuoteId
  type: string
- description: ''
  name: PricebookEntryId
  type: string
- description: ''
  name: Product2Id
  type: string
- description: ''
  name: Quantity
  type: number
- description: ''
  name: UnitPrice
  type: number
- description: ''
  name: PeriodBoundary
  type: string
- description: ''
  name: BillingFrequency
  type: string
- description: ''
  name: StartDate
  type: string
- description: ''
  name: EndDate
  type: string
- description: ''
  name: PeriodBoundaryDay
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record23-schema.json
slug: salesforce-record23
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"method\"\n      ]\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"Pricebook2Id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"QuoteId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"PricebookEntryId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"Product2Id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"Quantity\": {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"UnitPrice\"\
  : {\n      \"type\": \"number\",\n      \"example\": 42.5\n    },\n    \"PeriodBoundary\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"BillingFrequency\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"StartDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"EndDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"PeriodBoundaryDay\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"attributes\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Record23\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record23-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Record23
---
