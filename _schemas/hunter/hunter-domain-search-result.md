---
description: ''
layout: schema
name: DomainSearchResult
properties_list:
- description: The domain name searched.
  name: domain
  type: string
- description: Whether the domain is a disposable email service.
  name: disposable
  type: boolean
- description: Whether the domain is a webmail provider.
  name: webmail
  type: boolean
- description: Whether the mail server accepts all email addresses.
  name: accept_all
  type: boolean
- description: The email address pattern detected for the domain.
  name: pattern
  type: '[''string'', ''null'']'
- description: The name of the organization associated with the domain.
  name: organization
  type: string
- description: ''
  name: emails
  type: array
provider_name: Hunter
provider_slug: hunter
schema_file: json-schema/hunter-domain-search-result-schema.json
slug: hunter-domain-search-result
source_filename: hunter-domain-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DomainSearchResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"The domain name searched.\"\n    },\n    \"disposable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is a disposable email service.\"\n    },\n    \"webmail\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is a webmail provider.\"\n    },\n    \"accept_all\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the mail server accepts all email addresses.\"\n    },\n    \"pattern\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The email address pattern detected for the domain.\"\n    },\n    \"organization\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the organization associated with the domain.\"\n    },\n    \"emails\": {\n \
  \     \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hunter/refs/heads/main/json-schema/hunter-domain-search-result-schema.json
tags:
- Contact Discovery
- Email
- Email Verification
- Lead Generation
- Prospecting
- Sales Intelligence
title: DomainSearchResult
---
