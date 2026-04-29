---
description: Contains a key credential (certificate) associated with an application or service principal
layout: schema
name: KeyCredential
properties_list:
- description: Unique identifier for the key
  name: keyId
  type: string
- description: Friendly name for the key
  name: displayName
  type: '[''string'', ''null'']'
- description: Type of key credential
  name: type
  type: string
- description: Describes the purpose of the key
  name: usage
  type: string
- description: The certificate's raw data in byte array converted to Base64 string
  name: key
  type: string
- description: The date and time at which the credential becomes valid
  name: startDateTime
  type: string
- description: The date and time at which the credential expires
  name: endDateTime
  type: string
provider_name: Microsoft Entra
provider_slug: microsoft-entra
schema_file: json-schema/microsoft-entra-graph-identity-key-credential-schema.json
slug: microsoft-entra-graph-identity-key-credential
source_filename: microsoft-entra-graph-identity-key-credential-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyCredential\",\n  \"type\": \"object\",\n  \"description\": \"Contains a key credential (certificate) associated with an application or service principal\",\n  \"properties\": {\n    \"keyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the key\"\n    },\n    \"displayName\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Friendly name for the key\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of key credential\"\n    },\n    \"usage\": {\n      \"type\": \"string\",\n      \"description\": \"Describes the purpose of the key\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The certificate's raw data in byte array converted to Base64 string\"\n    },\n    \"startDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time at which the credential\
  \ becomes valid\"\n    },\n    \"endDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time at which the credential expires\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra/refs/heads/main/json-schema/microsoft-entra-graph-identity-key-credential-schema.json
tags:
- Access Management
- Authentication
- Azure AD
- Entra
- Identity
- Identity Governance
- Microsoft
- Network Security
- Security
- Zero Trust
title: KeyCredential
---
