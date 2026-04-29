---
description: An in-person signer recipient for face-to-face signing where a host manages the signing session.
layout: schema
name: InPersonSigner
properties_list:
- description: ''
  name: recipientId
  type: string
- description: The name of the signing host.
  name: hostName
  type: string
- description: The email of the signing host.
  name: hostEmail
  type: string
- description: The name of the in-person signer.
  name: signerName
  type: string
- description: The email of the in-person signer.
  name: signerEmail
  type: string
- description: ''
  name: routingOrder
  type: string
- description: ''
  name: status
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-in-person-signer-schema.json
slug: docusign-esignature-in-person-signer
source_filename: docusign-esignature-in-person-signer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InPersonSigner\",\n  \"type\": \"object\",\n  \"description\": \"An in-person signer recipient for face-to-face signing where a host manages the signing session.\",\n  \"properties\": {\n    \"recipientId\": {\n      \"type\": \"string\"\n    },\n    \"hostName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the signing host.\"\n    },\n    \"hostEmail\": {\n      \"type\": \"string\",\n      \"description\": \"The email of the signing host.\"\n    },\n    \"signerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the in-person signer.\"\n    },\n    \"signerEmail\": {\n      \"type\": \"string\",\n      \"description\": \"The email of the in-person signer.\"\n    },\n    \"routingOrder\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-in-person-signer-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: InPersonSigner
---
