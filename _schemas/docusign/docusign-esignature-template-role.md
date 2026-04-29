---
description: Maps a recipient to a role defined in a template. Used when creating an envelope from a template.
layout: schema
name: TemplateRole
properties_list:
- description: The recipient's full name.
  name: name
  type: string
- description: The recipient's email address.
  name: email
  type: string
- description: The role name that matches a role defined in the template.
  name: roleName
  type: string
- description: The client user ID for embedded signing.
  name: clientUserId
  type: string
- description: When true, this is the default recipient for the role.
  name: defaultRecipient
  type: string
- description: The routing order for the recipient.
  name: routingOrder
  type: string
- description: Access code for authentication.
  name: accessCode
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-template-role-schema.json
slug: docusign-esignature-template-role
source_filename: docusign-esignature-template-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TemplateRole\",\n  \"type\": \"object\",\n  \"description\": \"Maps a recipient to a role defined in a template. Used when creating an envelope from a template.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The recipient's full name.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The recipient's email address.\"\n    },\n    \"roleName\": {\n      \"type\": \"string\",\n      \"description\": \"The role name that matches a role defined in the template.\"\n    },\n    \"clientUserId\": {\n      \"type\": \"string\",\n      \"description\": \"The client user ID for embedded signing.\"\n    },\n    \"defaultRecipient\": {\n      \"type\": \"string\",\n      \"description\": \"When true, this is the default recipient for the role.\"\n    },\n    \"routingOrder\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The routing order for the recipient.\"\n    },\n    \"accessCode\": {\n      \"type\": \"string\",\n      \"description\": \"Access code for authentication.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-template-role-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: TemplateRole
---
