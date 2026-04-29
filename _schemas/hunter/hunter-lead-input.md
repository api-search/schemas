---
description: ''
layout: schema
name: LeadInput
properties_list:
- description: Email address of the lead.
  name: email
  type: string
- description: First name of the lead.
  name: first_name
  type: string
- description: Last name of the lead.
  name: last_name
  type: string
- description: Job position or title.
  name: position
  type: string
- description: Company name.
  name: company
  type: string
- description: Industry of the company.
  name: company_industry
  type: string
- description: Size range of the company.
  name: company_size
  type: string
- description: Confidence score for the lead email.
  name: confidence_score
  type: integer
- description: Website URL associated with the lead.
  name: website
  type: string
- description: ISO 3166-1 alpha-2 country code.
  name: country_code
  type: string
- description: LinkedIn profile URL.
  name: linkedin_url
  type: string
- description: Phone number.
  name: phone_number
  type: string
- description: Twitter handle.
  name: twitter
  type: string
- description: Free-text notes about the lead.
  name: notes
  type: string
- description: Identifier of the leads list to add the lead to.
  name: leads_list_id
  type: integer
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-lead-input-schema.json
slug: hunter-lead-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LeadInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address of the lead.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the lead.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the lead.\"\n    },\n    \"position\": {\n      \"type\": \"string\",\n      \"description\": \"Job position or title.\"\n    },\n    \"company\": {\n      \"type\": \"string\",\n      \"description\": \"Company name.\"\n    },\n    \"company_industry\": {\n      \"type\": \"string\",\n      \"description\": \"Industry of the company.\"\n    },\n    \"company_size\": {\n      \"type\": \"string\",\n      \"description\": \"Size range of the company.\"\n    },\n    \"confidence_score\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Confidence score for the lead email.\"\n    },\n    \"website\": {\n      \"type\": \"string\",\n      \"description\": \"Website URL associated with the lead.\"\n    },\n    \"country_code\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\"\n    },\n    \"linkedin_url\": {\n      \"type\": \"string\",\n      \"description\": \"LinkedIn profile URL.\"\n    },\n    \"phone_number\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number.\"\n    },\n    \"twitter\": {\n      \"type\": \"string\",\n      \"description\": \"Twitter handle.\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"Free-text notes about the lead.\"\n    },\n    \"leads_list_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Identifier of the leads list to add the lead to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-lead-input-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: LeadInput
---
