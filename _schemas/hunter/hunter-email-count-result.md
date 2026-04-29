---
description: ''
layout: schema
name: EmailCountResult
properties_list:
- description: Total number of email addresses found.
  name: total
  type: integer
- description: Number of personal email addresses.
  name: personal_emails
  type: integer
- description: Number of generic email addresses.
  name: generic_emails
  type: integer
- description: Breakdown of email count by department.
  name: department
  type: object
- description: Breakdown of email count by seniority level.
  name: seniority
  type: object
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-email-count-result-schema.json
slug: hunter-email-count-result
source_filename: hunter-email-count-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailCountResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of email addresses found.\"\n    },\n    \"personal_emails\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of personal email addresses.\"\n    },\n    \"generic_emails\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of generic email addresses.\"\n    },\n    \"department\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of email count by department.\"\n    },\n    \"seniority\": {\n      \"type\": \"object\",\n      \"description\": \"Breakdown of email count by seniority level.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-email-count-result-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: EmailCountResult
---
