---
description: ''
layout: schema
name: EmailFinderResult
properties_list:
- description: First name of the person.
  name: first_name
  type: string
- description: Last name of the person.
  name: last_name
  type: string
- description: The found email address.
  name: email
  type: string
- description: Confidence score for the email.
  name: score
  type: integer
- description: The domain name used for the search.
  name: domain
  type: string
- description: Job position or title.
  name: position
  type: '[''string'', ''null'']'
- description: Company name.
  name: company
  type: '[''string'', ''null'']'
- description: Twitter handle.
  name: twitter
  type: '[''string'', ''null'']'
- description: LinkedIn profile URL.
  name: linkedin_url
  type: '[''string'', ''null'']'
- description: Phone number.
  name: phone_number
  type: '[''string'', ''null'']'
- description: ''
  name: sources
  type: array
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-email-finder-result-schema.json
slug: hunter-email-finder-result
source_filename: hunter-email-finder-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailFinderResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the person.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the person.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The found email address.\"\n    },\n    \"score\": {\n      \"type\": \"integer\",\n      \"description\": \"Confidence score for the email.\"\n    },\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name used for the search.\"\n    },\n    \"position\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Job position or title.\"\n    },\n    \"company\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Company name.\"\n    },\n    \"twitter\": {\n      \"type\"\
  : \"['string', 'null']\",\n      \"description\": \"Twitter handle.\"\n    },\n    \"linkedin_url\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"LinkedIn profile URL.\"\n    },\n    \"phone_number\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Phone number.\"\n    },\n    \"sources\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-email-finder-result-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: EmailFinderResult
---
