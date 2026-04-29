---
description: A candidate in the recruiting pipeline from a connected ATS integration.
layout: schema
name: Candidate
properties_list:
- description: Unique Merge identifier.
  name: id
  type: string
- description: Third-party ID.
  name: remote_id
  type: string
- description: First name.
  name: first_name
  type: string
- description: Last name.
  name: last_name
  type: string
- description: Current or most recent company.
  name: company
  type: string
- description: Current or most recent title.
  name: title
  type: string
- description: Whether the candidate is private.
  name: is_private
  type: boolean
- description: Whether the candidate can be emailed.
  name: can_email
  type: boolean
- description: ''
  name: email_addresses
  type: array
- description: ''
  name: phone_numbers
  type: array
- description: ''
  name: tags
  type: array
- description: ''
  name: applications
  type: array
- description: ''
  name: attachments
  type: array
- description: ''
  name: remote_was_deleted
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: modified_at
  type: string
provider_name: Merge
provider_slug: merge
schema_file: json-schema/ats-api-candidate-schema.json
slug: ats-api-candidate
source_filename: ats-api-candidate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/ats-api-candidate-schema.json\",\n  \"title\": \"Candidate\",\n  \"description\": \"A candidate in the recruiting pipeline from a connected ATS integration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"format\": \"uuid\", \"description\": \"Unique Merge identifier.\" },\n    \"remote_id\": { \"type\": \"string\", \"description\": \"Third-party ID.\" },\n    \"first_name\": { \"type\": \"string\", \"description\": \"First name.\" },\n    \"last_name\": { \"type\": \"string\", \"description\": \"Last name.\" },\n    \"company\": { \"type\": \"string\", \"description\": \"Current or most recent company.\" },\n    \"title\": { \"type\": \"string\", \"description\": \"Current or most recent title.\" },\n    \"is_private\": { \"type\": \"boolean\", \"description\": \"Whether\
  \ the candidate is private.\" },\n    \"can_email\": { \"type\": \"boolean\", \"description\": \"Whether the candidate can be emailed.\" },\n    \"email_addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": { \"type\": \"string\", \"format\": \"email\" },\n          \"email_address_type\": { \"type\": \"string\", \"enum\": [\"PERSONAL\", \"WORK\", \"OTHER\"] }\n        }\n      }\n    },\n    \"phone_numbers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": { \"type\": \"string\" },\n          \"phone_number_type\": { \"type\": \"string\", \"enum\": [\"HOME\", \"WORK\", \"MOBILE\", \"SKYPE\", \"OTHER\"] }\n        }\n      }\n    },\n    \"tags\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n    \"applications\": { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uuid\" } },\n \
  \   \"attachments\": { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uuid\" } },\n    \"remote_was_deleted\": { \"type\": \"boolean\" },\n    \"created_at\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"modified_at\": { \"type\": \"string\", \"format\": \"date-time\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/merge/refs/heads/main/json-schema/ats-api-candidate-schema.json
tags:
- Integrations
- Platform
- Unified API
title: Candidate
---
