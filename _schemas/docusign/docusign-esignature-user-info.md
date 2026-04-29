---
description: Information about a DocuSign user.
layout: schema
name: UserInfo
properties_list:
- description: The user's full name.
  name: userName
  type: string
- description: The user's email address.
  name: email
  type: string
- description: The user's unique ID.
  name: userId
  type: string
- description: The account ID associated with the user.
  name: accountId
  type: string
provider_name: Docusign
provider_slug: docusign
schema_file: json-schema/docusign-esignature-user-info-schema.json
slug: docusign-esignature-user-info
source_filename: docusign-esignature-user-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserInfo\",\n  \"type\": \"object\",\n  \"description\": \"Information about a DocuSign user.\",\n  \"properties\": {\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"The user's full name.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"The user's email address.\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"The user's unique ID.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account ID associated with the user.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/docusign/refs/heads/main/json-schema/docusign-esignature-user-info-schema.json
tags:
- Agreements
- Contracts
- Digital Transaction Management
- Documents
- Electronic Signatures
- eSignature
title: UserInfo
---
