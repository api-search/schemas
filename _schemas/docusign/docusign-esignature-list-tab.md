---
description: A dropdown list tab for selecting from predefined options.
layout: schema
name: ListTab
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
- description: ''
  name: value
  type: string
- description: ''
  name: listItems
  type: array
- description: ''
  name: required
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-list-tab-schema.json
slug: docusign-esignature-list-tab
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTab\",\n  \"type\": \"object\",\n  \"description\": \"A dropdown list tab for selecting from predefined options.\",\n  \"properties\": {\n    \"tabId\": {\n      \"type\": \"string\"\n    },\n    \"tabLabel\": {\n      \"type\": \"string\"\n    },\n    \"documentId\": {\n      \"type\": \"string\"\n    },\n    \"pageNumber\": {\n      \"type\": \"string\"\n    },\n    \"recipientId\": {\n      \"type\": \"string\"\n    },\n    \"xPosition\": {\n      \"type\": \"string\"\n    },\n    \"yPosition\": {\n      \"type\": \"string\"\n    },\n    \"anchorString\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"listItems\": {\n      \"type\": \"array\"\n    },\n    \"required\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-list-tab-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: ListTab
---
