---
description: A decline button tab for document rejection.
layout: schema
name: Decline
properties_list:
- description: ''
  name: tabId
  type: string
- description: ''
  name: tabLabel
  type: string
- description: ''
  name: documentId
  type: string
- description: ''
  name: pageNumber
  type: string
- description: ''
  name: recipientId
  type: string
- description: ''
  name: xPosition
  type: string
- description: ''
  name: yPosition
  type: string
- description: ''
  name: buttonText
  type: string
- description: ''
  name: declineReason
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-decline-schema.json
slug: docusign-esignature-decline
source_filename: docusign-esignature-decline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Decline\",\n  \"type\": \"object\",\n  \"description\": \"A decline button tab for document rejection.\",\n  \"properties\": {\n    \"tabId\": {\n      \"type\": \"string\"\n    },\n    \"tabLabel\": {\n      \"type\": \"string\"\n    },\n    \"documentId\": {\n      \"type\": \"string\"\n    },\n    \"pageNumber\": {\n      \"type\": \"string\"\n    },\n    \"recipientId\": {\n      \"type\": \"string\"\n    },\n    \"xPosition\": {\n      \"type\": \"string\"\n    },\n    \"yPosition\": {\n      \"type\": \"string\"\n    },\n    \"buttonText\": {\n      \"type\": \"string\"\n    },\n    \"declineReason\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-decline-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: Decline
---
