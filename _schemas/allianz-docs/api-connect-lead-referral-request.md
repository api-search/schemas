---
description: Request body for submitting an instant lead referral to Allianz
layout: schema
name: LeadReferralRequest
properties_list:
- description: Full name of the customer being referred
  name: customer_name
  type: string
- description: Email address of the customer being referred
  name: customer_email
  type: string
- description: Phone number of the customer being referred
  name: customer_phone
  type: string
- description: Insurance product the customer is interested in
  name: product_type
  type: string
- description: Additional notes about the customer's insurance needs
  name: notes
  type: string
provider_name: Allianz
provider_slug: allianz-docs
schema_file: json-schema/api-connect-lead-referral-request-schema.json
slug: api-connect-lead-referral-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-lead-referral-request-schema.json\",\n  \"title\": \"LeadReferralRequest\",\n  \"description\": \"Request body for submitting an instant lead referral to Allianz\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customer_name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the customer being referred\",\n      \"example\": \"Jane Smith\"\n    },\n    \"customer_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the customer being referred\",\n      \"example\": \"jsmith@example.com\"\n    },\n    \"customer_phone\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number of the customer being referred\",\n      \"example\": \"+61400000000\"\n    },\n    \"product_type\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Insurance product the customer is interested in\",\n      \"enum\": [\n        \"home\",\n        \"landlord\",\n        \"car\"\n      ],\n      \"example\": \"home\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Additional notes about the customer's insurance needs\",\n      \"example\": \"Customer interested in home and contents for new property\"\n    }\n  },\n  \"required\": [\n    \"customer_name\",\n    \"customer_email\",\n    \"product_type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-docs/refs/heads/main/json-schema/api-connect-lead-referral-request-schema.json
tags:
- Financial Services
- Insurance
- Asset Management
title: LeadReferralRequest
---
