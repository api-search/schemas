---
description: A signer recipient who must sign the envelope documents.
layout: schema
name: Signer
properties_list:
- description: Unique identifier for the recipient. Assigned by the sender.
  name: recipientId
  type: string
- description: The GUID for the recipient.
  name: recipientIdGuid
  type: string
- description: The full legal name of the signer.
  name: name
  type: string
- description: The email address of the signer.
  name: email
  type: string
- description: The routing order of the signer. Lower numbers are processed first. Recipients with the same routing order sign in parallel.
  name: routingOrder
  type: string
- description: The role name associated with the signer, used with templates.
  name: roleName
  type: string
- description: The client user ID for embedded signing. When set, the recipient is an embedded signer and must sign through your application using a generated signing URL.
  name: clientUserId
  type: string
- description: The status of the signer.
  name: status
  type: string
- description: The date and time the signer signed.
  name: signedDateTime
  type: string
- description: The date and time the envelope was delivered to the signer.
  name: deliveredDateTime
  type: string
- description: The date and time the signer declined.
  name: declinedDateTime
  type: string
- description: The reason the signer declined.
  name: declinedReason
  type: string
- description: Identity verification settings for this recipient.
  name: identityVerification
  type: object
- description: Phone authentication settings.
  name: phoneAuthentication
  type: object
- description: An access code the recipient must enter to access the envelope.
  name: accessCode
  type: string
- description: Whether ID lookup authentication is required.
  name: requireIdLookup
  type: string
- description: A private note to the signer from the sender.
  name: note
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-signer-schema.json
slug: docusign-esignature-signer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Signer\",\n  \"type\": \"object\",\n  \"description\": \"A signer recipient who must sign the envelope documents.\",\n  \"properties\": {\n    \"recipientId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the recipient. Assigned by the sender.\"\n    },\n    \"recipientIdGuid\": {\n      \"type\": \"string\",\n      \"description\": \"The GUID for the recipient.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The full legal name of the signer.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the signer.\"\n    },\n    \"routingOrder\": {\n      \"type\": \"string\",\n      \"description\": \"The routing order of the signer. Lower numbers are processed first. Recipients with the same routing order sign in parallel.\"\n    },\n    \"roleName\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The role name associated with the signer, used with templates.\"\n    },\n    \"clientUserId\": {\n      \"type\": \"string\",\n      \"description\": \"The client user ID for embedded signing. When set, the recipient is an embedded signer and must sign through your application using a generated signing URL.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the signer.\"\n    },\n    \"signedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the signer signed.\"\n    },\n    \"deliveredDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the envelope was delivered to the signer.\"\n    },\n    \"declinedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the signer declined.\"\n    },\n    \"declinedReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the signer declined.\"\n    },\n\
  \    \"identityVerification\": {\n      \"type\": \"object\",\n      \"description\": \"Identity verification settings for this recipient.\"\n    },\n    \"phoneAuthentication\": {\n      \"type\": \"object\",\n      \"description\": \"Phone authentication settings.\"\n    },\n    \"accessCode\": {\n      \"type\": \"string\",\n      \"description\": \"An access code the recipient must enter to access the envelope.\"\n    },\n    \"requireIdLookup\": {\n      \"type\": \"string\",\n      \"description\": \"Whether ID lookup authentication is required.\"\n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"description\": \"A private note to the signer from the sender.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-signer-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: Signer
---
