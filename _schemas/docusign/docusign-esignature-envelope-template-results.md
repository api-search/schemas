---
description: Contains results of a template list request.
layout: schema
name: EnvelopeTemplateResults
properties_list:
- description: ''
  name: envelopeTemplates
  type: array
- description: ''
  name: resultSetSize
  type: string
- description: ''
  name: totalSetSize
  type: string
- description: ''
  name: startPosition
  type: string
- description: ''
  name: endPosition
  type: string
- description: ''
  name: nextUri
  type: string
- description: ''
  name: previousUri
  type: string
- description: ''
  name: folders
  type: array
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelope-template-results-schema.json
slug: docusign-esignature-envelope-template-results
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvelopeTemplateResults\",\n  \"type\": \"object\",\n  \"description\": \"Contains results of a template list request.\",\n  \"properties\": {\n    \"envelopeTemplates\": {\n      \"type\": \"array\"\n    },\n    \"resultSetSize\": {\n      \"type\": \"string\"\n    },\n    \"totalSetSize\": {\n      \"type\": \"string\"\n    },\n    \"startPosition\": {\n      \"type\": \"string\"\n    },\n    \"endPosition\": {\n      \"type\": \"string\"\n    },\n    \"nextUri\": {\n      \"type\": \"string\"\n    },\n    \"previousUri\": {\n      \"type\": \"string\"\n    },\n    \"folders\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelope-template-results-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EnvelopeTemplateResults
---
