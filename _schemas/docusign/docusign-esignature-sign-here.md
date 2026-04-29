---
description: A signature tab placed on a document.
layout: schema
name: SignHere
properties_list:
- description: Unique identifier for the tab.
  name: tabId
  type: string
- description: Label used to identify the tab.
  name: tabLabel
  type: string
- description: The document ID where this tab is placed.
  name: documentId
  type: string
- description: The page number where this tab is placed.
  name: pageNumber
  type: string
- description: The recipient this tab is assigned to.
  name: recipientId
  type: string
- description: The X position of the tab on the page.
  name: xPosition
  type: string
- description: The Y position of the tab on the page.
  name: yPosition
  type: string
- description: Anchor text string used to automatically position the tab.
  name: anchorString
  type: string
- description: X offset from the anchor string position.
  name: anchorXOffset
  type: string
- description: Y offset from the anchor string position.
  name: anchorYOffset
  type: string
- description: Units for anchor offsets (pixels, inches, mms, cms).
  name: anchorUnits
  type: string
- description: Scale value for the signature.
  name: scaleValue
  type: string
- description: When true, the tab is optional for the recipient.
  name: optional
  type: string
- description: The type of stamp for the signature.
  name: stampType
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-sign-here-schema.json
slug: docusign-esignature-sign-here
source_filename: docusign-esignature-sign-here-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SignHere\",\n  \"type\": \"object\",\n  \"description\": \"A signature tab placed on a document.\",\n  \"properties\": {\n    \"tabId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the tab.\"\n    },\n    \"tabLabel\": {\n      \"type\": \"string\",\n      \"description\": \"Label used to identify the tab.\"\n    },\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"The document ID where this tab is placed.\"\n    },\n    \"pageNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The page number where this tab is placed.\"\n    },\n    \"recipientId\": {\n      \"type\": \"string\",\n      \"description\": \"The recipient this tab is assigned to.\"\n    },\n    \"xPosition\": {\n      \"type\": \"string\",\n      \"description\": \"The X position of the tab on the page.\"\n    },\n    \"yPosition\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The Y position of the tab on the page.\"\n    },\n    \"anchorString\": {\n      \"type\": \"string\",\n      \"description\": \"Anchor text string used to automatically position the tab.\"\n    },\n    \"anchorXOffset\": {\n      \"type\": \"string\",\n      \"description\": \"X offset from the anchor string position.\"\n    },\n    \"anchorYOffset\": {\n      \"type\": \"string\",\n      \"description\": \"Y offset from the anchor string position.\"\n    },\n    \"anchorUnits\": {\n      \"type\": \"string\",\n      \"description\": \"Units for anchor offsets (pixels, inches, mms, cms).\"\n    },\n    \"scaleValue\": {\n      \"type\": \"string\",\n      \"description\": \"Scale value for the signature.\"\n    },\n    \"optional\": {\n      \"type\": \"string\",\n      \"description\": \"When true, the tab is optional for the recipient.\"\n    },\n    \"stampType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of stamp for\
  \ the signature.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-sign-here-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: SignHere
---
