---
description: A document to be included in an envelope. Documents can be provided as base64-encoded content or by reference.
layout: schema
name: Document
properties_list:
- description: A unique identifier for the document within the envelope, assigned by the sender. Must be unique within the envelope.
  name: documentId
  type: string
- description: The name of the document.
  name: name
  type: string
- description: The file extension of the document. DocuSign uses this to determine the correct content type.
  name: fileExtension
  type: string
- description: The base64-encoded content of the document.
  name: documentBase64
  type: string
- description: URL from which to retrieve the document content.
  name: remoteUrl
  type: string
- description: The order of the document in the envelope.
  name: order
  type: string
- description: The number of pages in the document.
  name: pages
  type: string
- description: Display setting for the document.
  name: display
  type: string
- description: Whether to include this document in downloads.
  name: includeInDownload
  type: string
- description: When true, DocuSign transforms PDF form fields into DocuSign tabs.
  name: transformPdfFields
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-document-schema.json
slug: docusign-esignature-document
source_filename: docusign-esignature-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Document\",\n  \"type\": \"object\",\n  \"description\": \"A document to be included in an envelope. Documents can be provided as base64-encoded content or by reference.\",\n  \"properties\": {\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the document within the envelope, assigned by the sender. Must be unique within the envelope.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the document.\"\n    },\n    \"fileExtension\": {\n      \"type\": \"string\",\n      \"description\": \"The file extension of the document. DocuSign uses this to determine the correct content type.\"\n    },\n    \"documentBase64\": {\n      \"type\": \"string\",\n      \"description\": \"The base64-encoded content of the document.\"\n    },\n    \"remoteUrl\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"URL from which to retrieve the document content.\"\n    },\n    \"order\": {\n      \"type\": \"string\",\n      \"description\": \"The order of the document in the envelope.\"\n    },\n    \"pages\": {\n      \"type\": \"string\",\n      \"description\": \"The number of pages in the document.\"\n    },\n    \"display\": {\n      \"type\": \"string\",\n      \"description\": \"Display setting for the document.\"\n    },\n    \"includeInDownload\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to include this document in downloads.\"\n    },\n    \"transformPdfFields\": {\n      \"type\": \"string\",\n      \"description\": \"When true, DocuSign transforms PDF form fields into DocuSign tabs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-document-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: Document
---
