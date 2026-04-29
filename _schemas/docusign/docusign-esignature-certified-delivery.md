---
description: A certified delivery recipient who must confirm receipt of the envelope documents.
layout: schema
name: CertifiedDelivery
properties_list:
- description: ''
  name: recipientId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: routingOrder
  type: string
- description: ''
  name: status
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-certified-delivery-schema.json
slug: docusign-esignature-certified-delivery
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertifiedDelivery\",\n  \"type\": \"object\",\n  \"description\": \"A certified delivery recipient who must confirm receipt of the envelope documents.\",\n  \"properties\": {\n    \"recipientId\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"routingOrder\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-certified-delivery-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: CertifiedDelivery
---
