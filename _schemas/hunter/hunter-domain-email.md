---
description: ''
layout: schema
name: DomainEmail
properties_list:
- description: The email address.
  name: value
  type: string
- description: Whether the email is personal or generic.
  name: type
  type: string
- description: Confidence score for the email address.
  name: confidence
  type: integer
- description: First name of the person.
  name: first_name
  type: '[''string'', ''null'']'
- description: Last name of the person.
  name: last_name
  type: '[''string'', ''null'']'
- description: Job position or title.
  name: position
  type: '[''string'', ''null'']'
- description: Seniority level.
  name: seniority
  type: '[''string'', ''null'']'
- description: Department within the organization.
  name: department
  type: '[''string'', ''null'']'
- description: LinkedIn profile URL.
  name: linkedin
  type: '[''string'', ''null'']'
- description: Twitter handle.
  name: twitter
  type: '[''string'', ''null'']'
- description: Phone number.
  name: phone_number
  type: '[''string'', ''null'']'
- description: ''
  name: sources
  type: array
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-domain-email-schema.json
slug: hunter-domain-email
source_filename: hunter-domain-email-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DomainEmail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The email address.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the email is personal or generic.\"\n    },\n    \"confidence\": {\n      \"type\": \"integer\",\n      \"description\": \"Confidence score for the email address.\"\n    },\n    \"first_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"First name of the person.\"\n    },\n    \"last_name\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Last name of the person.\"\n    },\n    \"position\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Job position or title.\"\n    },\n    \"seniority\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Seniority level.\"\n    },\n\
  \    \"department\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Department within the organization.\"\n    },\n    \"linkedin\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"LinkedIn profile URL.\"\n    },\n    \"twitter\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Twitter handle.\"\n    },\n    \"phone_number\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Phone number.\"\n    },\n    \"sources\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-domain-email-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: DomainEmail
---
