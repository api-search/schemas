---
description: Contains the list of documents in an envelope.
layout: schema
name: EnvelopeDocumentsResult
properties_list:
- description: The envelope ID.
  name: envelopeId
  type: string
- description: The list of envelope documents.
  name: envelopeDocuments
  type: array
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelope-documents-result-schema.json
slug: docusign-esignature-envelope-documents-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvelopeDocumentsResult\",\n  \"type\": \"object\",\n  \"description\": \"Contains the list of documents in an envelope.\",\n  \"properties\": {\n    \"envelopeId\": {\n      \"type\": \"string\",\n      \"description\": \"The envelope ID.\"\n    },\n    \"envelopeDocuments\": {\n      \"type\": \"array\",\n      \"description\": \"The list of envelope documents.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelope-documents-result-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EnvelopeDocumentsResult
---
