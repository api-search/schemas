---
description: Contains a key credential (certificate) associated with an application or service principal.
layout: schema
name: KeyCredential
properties_list:
- description: Custom key identifier.
  name: customKeyIdentifier
  type: '[''string'', ''null'']'
- description: ''
  name: displayName
  type: '[''string'', ''null'']'
- description: The date and time at which the credential expires.
  name: endDateTime
  type: string
- description: The certificate raw data in byte array converted to Base64 string.
  name: key
  type: '[''string'', ''null'']'
- description: ''
  name: keyId
  type: string
- description: ''
  name: startDateTime
  type: string
- description: The type of key credential (e.g., AsymmetricX509Cert).
  name: type
  type: string
- description: Describes the purpose of the key. Valid values are Verify and Sign.
  name: usage
  type: string
provider_name: Azure Active Directory
provider_slug: azure-active-directory
schema_file: json-schema/microsoft-graph-identity-key-credential-schema.json
slug: microsoft-graph-identity-key-credential
source_filename: microsoft-graph-identity-key-credential-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KeyCredential\",\n  \"type\": \"object\",\n  \"description\": \"Contains a key credential (certificate) associated with an application or service principal.\",\n  \"properties\": {\n    \"customKeyIdentifier\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"Custom key identifier.\"\n    },\n    \"displayName\": {\n      \"type\": \"['string', 'null']\"\n    },\n    \"endDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time at which the credential expires.\"\n    },\n    \"key\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The certificate raw data in byte array converted to Base64 string.\"\n    },\n    \"keyId\": {\n      \"type\": \"string\"\n    },\n    \"startDateTime\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of key credential (e.g.,\
  \ AsymmetricX509Cert).\"\n    },\n    \"usage\": {\n      \"type\": \"string\",\n      \"description\": \"Describes the purpose of the key. Valid values are Verify and Sign.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-key-credential-schema.json
tags:
- Authentication
- Authorization
- Identity
- Microsoft
- Microsoft Entra
- OAuth
- OpenID Connect
- SAML
- SCIM
- Single Sign-On
- Zero Trust
title: KeyCredential
---
