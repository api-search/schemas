---
description: ''
layout: schema
name: Lead
properties_list:
- description: Unique identifier for the lead.
  name: id
  type: integer
- description: Email address of the lead.
  name: email
  type: string
- description: First name of the lead.
  name: first_name
  type: '[''string'', ''null'']'
- description: Last name of the lead.
  name: last_name
  type: '[''string'', ''null'']'
- description: Job position or title.
  name: position
  type: '[''string'', ''null'']'
- description: Company name.
  name: company
  type: '[''string'', ''null'']'
- description: Industry of the company.
  name: company_industry
  type: '[''string'', ''null'']'
- description: Size range of the company.
  name: company_size
  type: '[''string'', ''null'']'
- description: Confidence score for the lead email.
  name: confidence_score
  type: '[''integer'', ''null'']'
- description: Website URL associated with the lead.
  name: website
  type: '[''string'', ''null'']'
- description: ISO 3166-1 alpha-2 country code.
  name: country_code
  type: '[''string'', ''null'']'
- description: LinkedIn profile URL.
  name: linkedin_url
  type: '[''string'', ''null'']'
- description: Phone number.
  name: phone_number
  type: '[''string'', ''null'']'
- description: Twitter handle.
  name: twitter
  type: '[''string'', ''null'']'
- description: Free-text notes about the lead.
  name: notes
  type: '[''string'', ''null'']'
- description: Identifier of the leads list the lead belongs to.
  name: leads_list_id
  type: '[''integer'', ''null'']'
- description: CRM synchronization status.
  name: sync_status
  type: '[''string'', ''null'']'
- description: Email sending status.
  name: sending_status
  type: '[''string'', ''null'']'
- description: Timestamp of the last activity for this lead.
  name: last_activity_at
  type: '[''string'', ''null'']'
- description: Timestamp of the last contact with this lead.
  name: last_contacted_at
  type: '[''string'', ''null'']'
- description: Timestamp when the lead was created.
  name: created_at
  type: string
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-lead-schema.json
slug: hunter-lead
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Lead\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the lead.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address of the lead.\"\n    },\n    \"first_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"First name of the lead.\"\n    },\n    \"last_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Last name of the lead.\"\n    },\n    \"position\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Job position or title.\"\n    },\n    \"company\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Company name.\"\n    },\n    \"company_industry\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Industry of the company.\"\n    },\n    \"company_size\"\
  : {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Size range of the company.\"\n    },\n    \"confidence_score\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Confidence score for the lead email.\"\n    },\n    \"website\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Website URL associated with the lead.\"\n    },\n    \"country_code\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"ISO 3166-1 alpha-2 country code.\"\n    },\n    \"linkedin_url\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"LinkedIn profile URL.\"\n    },\n    \"phone_number\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Phone number.\"\n    },\n    \"twitter\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Twitter handle.\"\n    },\n    \"notes\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Free-text notes about the lead.\"\n    },\n\
  \    \"leads_list_id\": {\n      \"type\": \"['integer', 'null']\",\n      \"description\": \"Identifier of the leads list the lead belongs to.\"\n    },\n    \"sync_status\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"CRM synchronization status.\"\n    },\n    \"sending_status\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Email sending status.\"\n    },\n    \"last_activity_at\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Timestamp of the last activity for this lead.\"\n    },\n    \"last_contacted_at\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Timestamp of the last contact with this lead.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the lead was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-lead-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: Lead
---
