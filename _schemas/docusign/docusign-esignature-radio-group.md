---
description: A group of radio buttons for single-choice selection.
layout: schema
name: RadioGroup
properties_list:
- description: The name of the radio group.
  name: groupName
  type: string
- description: ''
  name: documentId
  type: string
- description: ''
  name: recipientId
  type: string
- description: ''
  name: radios
  type: array
- description: ''
  name: required
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-radio-group-schema.json
slug: docusign-esignature-radio-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RadioGroup\",\n  \"type\": \"object\",\n  \"description\": \"A group of radio buttons for single-choice selection.\",\n  \"properties\": {\n    \"groupName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the radio group.\"\n    },\n    \"documentId\": {\n      \"type\": \"string\"\n    },\n    \"recipientId\": {\n      \"type\": \"string\"\n    },\n    \"radios\": {\n      \"type\": \"array\"\n    },\n    \"required\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-radio-group-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: RadioGroup
---
