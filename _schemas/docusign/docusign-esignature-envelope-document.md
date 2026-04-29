---
description: Metadata about a document within an envelope.
layout: schema
name: EnvelopeDocument
properties_list:
- description: The unique identifier of the document.
  name: documentId
  type: string
- description: The name of the document.
  name: name
  type: string
- description: The document type.
  name: type
  type: string
- description: URI for retrieving the document.
  name: uri
  type: string
- description: The order of the document in the envelope.
  name: order
  type: string
- description: Array of page objects for the document.
  name: pages
  type: array
- description: Whether the document contains PDF form fields.
  name: containsPdfFormFields
  type: string
- description: Display setting for the document.
  name: display
  type: string
- description: Whether to include this document in downloads.
  name: includeInDownload
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-envelope-document-schema.json
slug: docusign-esignature-envelope-document
source_filename: docusign-esignature-envelope-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EnvelopeDocument\",\n  \"type\": \"object\",\n  \"description\": \"Metadata about a document within an envelope.\",\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the document.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the document.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The document type.\"\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"description\": \"URI for retrieving the document.\"\n    },\n    \"order\": {\n      \"type\": \"string\",\n      \"description\": \"The order of the document in the envelope.\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"description\": \"Array of page objects for the document.\"\n    },\n    \"containsPdfFormFields\": {\n      \"type\": \"string\",\n    \
  \  \"description\": \"Whether the document contains PDF form fields.\"\n    },\n    \"display\": {\n      \"type\": \"string\",\n      \"description\": \"Display setting for the document.\"\n    },\n    \"includeInDownload\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to include this document in downloads.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-envelope-document-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: EnvelopeDocument
---
