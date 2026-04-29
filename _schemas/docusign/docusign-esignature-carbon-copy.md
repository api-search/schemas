---
description: A carbon copy recipient who receives a copy of the completed documents but does not need to take any action.
layout: schema
name: CarbonCopy
properties_list:
- description: Unique identifier for the recipient.
  name: recipientId
  type: string
- description: The full name of the recipient.
  name: name
  type: string
- description: The email address of the recipient.
  name: email
  type: string
- description: The routing order of the recipient.
  name: routingOrder
  type: string
- description: The role name for template matching.
  name: roleName
  type: string
- description: The status of the recipient.
  name: status
  type: string
- description: A note for the recipient.
  name: note
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-carbon-copy-schema.json
slug: docusign-esignature-carbon-copy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CarbonCopy\",\n  \"type\": \"object\",\n  \"description\": \"A carbon copy recipient who receives a copy of the completed documents but does not need to take any action.\",\n  \"properties\": {\n    \"recipientId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the recipient.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the recipient.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the recipient.\"\n    },\n    \"routingOrder\": {\n      \"type\": \"string\",\n      \"description\": \"The routing order of the recipient.\"\n    },\n    \"roleName\": {\n      \"type\": \"string\",\n      \"description\": \"The role name for template matching.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the recipient.\"\
  \n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"description\": \"A note for the recipient.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-carbon-copy-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: CarbonCopy
---
