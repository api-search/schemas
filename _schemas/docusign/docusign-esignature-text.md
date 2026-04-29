---
description: A text input tab for free-form text entry.
layout: schema
name: Text
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
- description: When true, the recipient must fill in this tab.
  name: required
  type: string
- description: When true, the tab value cannot be changed.
  name: locked
  type: string
- description: Maximum length of text input.
  name: maxLength
  type: string
- description: ''
  name: width
  type: string
- description: ''
  name: height
  type: string
- description: ''
  name: font
  type: string
- description: ''
  name: fontSize
  type: string
- description: ''
  name: fontColor
  type: string
- description: ''
  name: bold
  type: string
- description: ''
  name: italic
  type: string
- description: ''
  name: underline
  type: string
- description: Regular expression for input validation.
  name: validationPattern
  type: string
- description: Error message displayed when validation fails.
  name: validationMessage
  type: string
- description: When true, the value is concealed on the document.
  name: concealValueOnDocument
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-text-schema.json
slug: docusign-esignature-text
source_filename: docusign-esignature-text-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Text\",\n  \"type\": \"object\",\n  \"description\": \"A text input tab for free-form text entry.\",\n  \"properties\": {\n    \"tabId\": {\n      \"type\": \"string\"\n    },\n    \"tabLabel\": {\n      \"type\": \"string\"\n    },\n    \"documentId\": {\n      \"type\": \"string\"\n    },\n    \"pageNumber\": {\n      \"type\": \"string\"\n    },\n    \"recipientId\": {\n      \"type\": \"string\"\n    },\n    \"xPosition\": {\n      \"type\": \"string\"\n    },\n    \"yPosition\": {\n      \"type\": \"string\"\n    },\n    \"anchorString\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"required\": {\n      \"type\": \"string\",\n      \"description\": \"When true, the recipient must fill in this tab.\"\n    },\n    \"locked\": {\n      \"type\": \"string\",\n      \"description\": \"When true, the tab value cannot be changed.\"\n    },\n\
  \    \"maxLength\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum length of text input.\"\n    },\n    \"width\": {\n      \"type\": \"string\"\n    },\n    \"height\": {\n      \"type\": \"string\"\n    },\n    \"font\": {\n      \"type\": \"string\"\n    },\n    \"fontSize\": {\n      \"type\": \"string\"\n    },\n    \"fontColor\": {\n      \"type\": \"string\"\n    },\n    \"bold\": {\n      \"type\": \"string\"\n    },\n    \"italic\": {\n      \"type\": \"string\"\n    },\n    \"underline\": {\n      \"type\": \"string\"\n    },\n    \"validationPattern\": {\n      \"type\": \"string\",\n      \"description\": \"Regular expression for input validation.\"\n    },\n    \"validationMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error message displayed when validation fails.\"\n    },\n    \"concealValueOnDocument\": {\n      \"type\": \"string\",\n      \"description\": \"When true, the value is concealed on the document.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-text-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: Text
---
