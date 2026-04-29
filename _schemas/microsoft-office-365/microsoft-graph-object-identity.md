---
description: Represents an identity used to sign in to a user account.
layout: schema
name: ObjectIdentity
properties_list:
- description: Specifies the type of user sign-in (e.g. emailAddress, userName, userPrincipalName).
  name: signInType
  type: string
- description: Specifies the issuer of the identity, for example contoso.onmicrosoft.com.
  name: issuer
  type: string
- description: Specifies the unique value associated with the issuer- signInType combination.
  name: issuerAssignedId
  type: string
provider_name: Microsoft Office 365
provider_slug: microsoft-office-365
schema_file: json-schema/microsoft-graph-object-identity-schema.json
slug: microsoft-graph-object-identity
source_filename: microsoft-graph-object-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectIdentity\",\n  \"type\": \"object\",\n  \"description\": \"Represents an identity used to sign in to a user account.\",\n  \"properties\": {\n    \"signInType\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the type of user sign-in (e.g. emailAddress, userName, userPrincipalName).\"\n    },\n    \"issuer\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the issuer of the identity, for example contoso.onmicrosoft.com.\"\n    },\n    \"issuerAssignedId\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the unique value associated with the issuer- signInType combination.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-365/refs/heads/main/json-schema/microsoft-graph-object-identity-schema.json
tags:
- Cloud
- Collaboration
- Enterprise
- Microsoft
- Productivity
title: ObjectIdentity
---
