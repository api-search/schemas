---
description: Contains error information returned by the API.
layout: schema
name: ErrorDetails
properties_list:
- description: The error code.
  name: errorCode
  type: string
- description: A human-readable error message.
  name: message
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-error-details-schema.json
slug: docusign-esignature-error-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetails\",\n  \"type\": \"object\",\n  \"description\": \"Contains error information returned by the API.\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-error-details-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: ErrorDetails
---
