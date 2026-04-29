---
description: ''
layout: schema
name: EmailVerifierResult
properties_list:
- description: The verification status of the email address.
  name: status
  type: string
- description: Deprecated. The deliverability result.
  name: result
  type: string
- description: Deliverability score.
  name: score
  type: integer
- description: The email address that was verified.
  name: email
  type: string
- description: Whether the email matches a valid format.
  name: regexp
  type: boolean
- description: Whether the email appears to be gibberish.
  name: gibberish
  type: boolean
- description: Whether the email uses a disposable provider.
  name: disposable
  type: boolean
- description: Whether the email is a webmail address.
  name: webmail
  type: boolean
- description: Whether MX records exist for the domain.
  name: mx_records
  type: boolean
- description: Whether an SMTP server was found.
  name: smtp_server
  type: boolean
- description: Whether the SMTP check passed.
  name: smtp_check
  type: boolean
- description: Whether the mail server accepts all addresses.
  name: accept_all
  type: boolean
- description: Whether the email is blocked.
  name: block
  type: boolean
- description: ''
  name: sources
  type: array
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-email-verifier-result-schema.json
slug: hunter-email-verifier-result
source_filename: hunter-email-verifier-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailVerifierResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The verification status of the email address.\"\n    },\n    \"result\": {\n      \"type\": \"string\",\n      \"description\": \"Deprecated. The deliverability result.\"\n    },\n    \"score\": {\n      \"type\": \"integer\",\n      \"description\": \"Deliverability score.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address that was verified.\"\n    },\n    \"regexp\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email matches a valid format.\"\n    },\n    \"gibberish\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email appears to be gibberish.\"\n    },\n    \"disposable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email uses\
  \ a disposable provider.\"\n    },\n    \"webmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email is a webmail address.\"\n    },\n    \"mx_records\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether MX records exist for the domain.\"\n    },\n    \"smtp_server\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether an SMTP server was found.\"\n    },\n    \"smtp_check\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the SMTP check passed.\"\n    },\n    \"accept_all\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the mail server accepts all addresses.\"\n    },\n    \"block\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the email is blocked.\"\n    },\n    \"sources\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-email-verifier-result-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: EmailVerifierResult
---
