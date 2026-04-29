---
description: Summary information about a newly created envelope.
layout: schema
name: EnvelopeSummary
properties_list:
- description: The unique identifier of the created envelope.
  name: envelopeId
  type: string
- description: The URI for the envelope.
  name: uri
  type: string
- description: The date and time of the status change.
  name: statusDateTime
  type: string
- description: The status of the envelope.
  name: status
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelope-summary-schema.json
slug: docusign-esignature-envelope-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvelopeSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary information about a newly created envelope.\",\n  \"properties\": {\n    \"envelopeId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the created envelope.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"The URI for the envelope.\"\n    },\n    \"statusDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time of the status change.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the envelope.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelope-summary-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EnvelopeSummary
---
