---
description: ''
layout: schema
name: ProtectPDFRequest
properties_list:
- description: The asset ID of the PDF to protect.
  name: assetID
  type: string
- description: ''
  name: passwordProtection
  type: object
- description: The encryption algorithm to use.
  name: encryptionAlgorithm
  type: string
- description: Permissions to set on the protected document.
  name: permissions
  type: object
provider_name: Adobe
provider_slug: adobe
schema_file: json-schema/adobe-pdf-services-protect-pdf-request-schema.json
slug: adobe-pdf-services-protect-pdf-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProtectPDFRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetID\": {\n      \"type\": \"string\",\n      \"description\": \"The asset ID of the PDF to protect.\"\n    },\n    \"passwordProtection\": {\n      \"type\": \"object\"\n    },\n    \"encryptionAlgorithm\": {\n      \"type\": \"string\",\n      \"description\": \"The encryption algorithm to use.\"\n    },\n    \"permissions\": {\n      \"type\": \"object\",\n      \"description\": \"Permissions to set on the protected document.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe/refs/heads/main/json-schema/adobe-pdf-services-protect-pdf-request-schema.json
tags:
- Analytics
- Creative Cloud
- Digital Asset Management
- Document Services
- E-Commerce
- E-Signatures
- Experience Cloud
- Generative AI
- Marketing
- PDF
- Work Management
title: ProtectPDFRequest
---
