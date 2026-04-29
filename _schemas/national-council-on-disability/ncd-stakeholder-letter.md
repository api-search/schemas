---
description: A formal letter from the National Council on Disability to a federal agency, congressional leader, or other government stakeholder.
layout: schema
name: NCD Stakeholder Letter
properties_list:
- description: Letter title or subject
  name: title
  type: string
- description: Date the letter was sent
  name: date
  type: string
- description: Name or office of the letter recipient
  name: recipient
  type: string
- description: Federal agency or organization of the recipient
  name: recipientAgency
  type: string
- description: Subject matter of the letter
  name: subject
  type: string
- description: Primary disability policy area addressed
  name: policyArea
  type: string
- description: URL to the full letter document
  name: documentURL
  type: string
provider_name: National Council on Disability
provider_slug: national-council-on-disability
schema_file: json-schema/ncd-stakeholder-letter-schema.json
slug: ncd-stakeholder-letter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.ncd.gov/schemas/stakeholder-letter\",\n  \"title\": \"NCD Stakeholder Letter\",\n  \"description\": \"A formal letter from the National Council on Disability to a federal agency, congressional leader, or other government stakeholder.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"title\",\n    \"date\",\n    \"recipient\"\n  ],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Letter title or subject\"\n    },\n    \"date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date the letter was sent\"\n    },\n    \"recipient\": {\n      \"type\": \"string\",\n      \"description\": \"Name or office of the letter recipient\"\n    },\n    \"recipientAgency\": {\n      \"type\": \"string\",\n      \"description\": \"Federal agency or organization of the recipient\"\n    },\n    \"subject\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"Subject matter of the letter\"\n    },\n    \"policyArea\": {\n      \"type\": \"string\",\n      \"description\": \"Primary disability policy area addressed\"\n    },\n    \"documentURL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the full letter document\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/national-council-on-disability/refs/heads/main/json-schema/ncd-stakeholder-letter-schema.json
tags:
- Disability
- Federal Government
- Policy
- Civil Rights
- Healthcare
- Independent Agency
title: NCD Stakeholder Letter
---
