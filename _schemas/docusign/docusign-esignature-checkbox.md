---
description: A checkbox tab for boolean selection.
layout: schema
name: Checkbox
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
  name: anchorString
  type: string
- description: When true, the checkbox is selected.
  name: selected
  type: string
- description: ''
  name: required
  type: string
- description: ''
  name: locked
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-checkbox-schema.json
slug: docusign-esignature-checkbox
source_filename: docusign-esignature-checkbox-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Checkbox\",\n  \"type\": \"object\",\n  \"description\": \"A checkbox tab for boolean selection.\",\n  \"properties\": {\n    \"tabId\": {\n      \"type\": \"string\"\n    },\n    \"tabLabel\": {\n      \"type\": \"string\"\n    },\n    \"documentId\": {\n      \"type\": \"string\"\n    },\n    \"pageNumber\": {\n      \"type\": \"string\"\n    },\n    \"recipientId\": {\n      \"type\": \"string\"\n    },\n    \"xPosition\": {\n      \"type\": \"string\"\n    },\n    \"yPosition\": {\n      \"type\": \"string\"\n    },\n    \"anchorString\": {\n      \"type\": \"string\"\n    },\n    \"selected\": {\n      \"type\": \"string\",\n      \"description\": \"When true, the checkbox is selected.\"\n    },\n    \"required\": {\n      \"type\": \"string\"\n    },\n    \"locked\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-checkbox-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: Checkbox
---
