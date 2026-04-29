---
description: Request body for generating an embedded recipient signing URL.
layout: schema
name: RecipientViewRequest
properties_list:
- description: The authentication method used to verify the recipient. Must match the authentication method used when the recipient was added.
  name: authenticationMethod
  type: string
- description: The email address of the recipient.
  name: email
  type: string
- description: The full name of the recipient.
  name: userName
  type: string
- description: The client user ID of the embedded signer.
  name: clientUserId
  type: string
- description: The recipient ID.
  name: recipientId
  type: string
- description: The URL to redirect the signer to after the signing session ends. DocuSign appends event query parameters.
  name: returnUrl
  type: string
- description: A URL that DocuSign pings during the signing session to confirm the parent frame is active.
  name: pingUrl
  type: string
- description: Frequency in seconds for ping requests.
  name: pingFrequency
  type: string
- description: URLs allowed to iframe the signing session (CSP frame-ancestors).
  name: frameAncestors
  type: array
- description: Origins allowed to receive postMessage events.
  name: messageOrigins
  type: array
- description: The security domain for the signing session.
  name: securityDomain
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-recipient-view-request-schema.json
slug: docusign-esignature-recipient-view-request
source_filename: docusign-esignature-recipient-view-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecipientViewRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for generating an embedded recipient signing URL.\",\n  \"properties\": {\n    \"authenticationMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication method used to verify the recipient. Must match the authentication method used when the recipient was added.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the recipient.\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the recipient.\"\n    },\n    \"clientUserId\": {\n      \"type\": \"string\",\n      \"description\": \"The client user ID of the embedded signer.\"\n    },\n    \"recipientId\": {\n      \"type\": \"string\",\n      \"description\": \"The recipient ID.\"\n    },\n    \"returnUrl\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The URL to redirect the signer to after the signing session ends. DocuSign appends event query parameters.\"\n    },\n    \"pingUrl\": {\n      \"type\": \"string\",\n      \"description\": \"A URL that DocuSign pings during the signing session to confirm the parent frame is active.\"\n    },\n    \"pingFrequency\": {\n      \"type\": \"string\",\n      \"description\": \"Frequency in seconds for ping requests.\"\n    },\n    \"frameAncestors\": {\n      \"type\": \"array\",\n      \"description\": \"URLs allowed to iframe the signing session (CSP frame-ancestors).\"\n    },\n    \"messageOrigins\": {\n      \"type\": \"array\",\n      \"description\": \"Origins allowed to receive postMessage events.\"\n    },\n    \"securityDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The security domain for the signing session.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-recipient-view-request-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: RecipientViewRequest
---
