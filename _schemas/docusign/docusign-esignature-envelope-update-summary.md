---
description: Summary of an envelope update operation.
layout: schema
name: EnvelopeUpdateSummary
properties_list:
- description: The envelope ID.
  name: envelopeId
  type: string
- description: Bulk envelope status information, if applicable.
  name: bulkEnvelopeStatus
  type: object
- description: ''
  name: listCustomFieldUpdateResults
  type: array
- description: ''
  name: recipientUpdateResults
  type: array
- description: ''
  name: textCustomFieldUpdateResults
  type: array
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelope-update-summary-schema.json
slug: docusign-esignature-envelope-update-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvelopeUpdateSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of an envelope update operation.\",\n  \"properties\": {\n    \"envelopeId\": {\n      \"type\": \"string\",\n      \"description\": \"The envelope ID.\"\n    },\n    \"bulkEnvelopeStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Bulk envelope status information, if applicable.\"\n    },\n    \"listCustomFieldUpdateResults\": {\n      \"type\": \"array\"\n    },\n    \"recipientUpdateResults\": {\n      \"type\": \"array\"\n    },\n    \"textCustomFieldUpdateResults\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelope-update-summary-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EnvelopeUpdateSummary
---
