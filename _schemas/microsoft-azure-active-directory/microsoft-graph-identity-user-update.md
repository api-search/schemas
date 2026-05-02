---
description: Properties that can be updated on an existing user.
layout: schema
name: UserUpdate
properties_list:
- description: ''
  name: accountEnabled
  type: boolean
- description: ''
  name: displayName
  type: string
- description: ''
  name: givenName
  type: string
- description: ''
  name: surname
  type: string
- description: ''
  name: jobTitle
  type: string
- description: ''
  name: department
  type: string
- description: ''
  name: mail
  type: string
- description: ''
  name: mobilePhone
  type: string
- description: ''
  name: businessPhones
  type: array
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: country
  type: string
- description: ''
  name: postalCode
  type: string
- description: ''
  name: streetAddress
  type: string
- description: ''
  name: officeLocation
  type: string
- description: ''
  name: usageLocation
  type: string
- description: ''
  name: preferredLanguage
  type: string
- description: ''
  name: employeeId
  type: string
- description: ''
  name: employeeType
  type: string
- description: ''
  name: companyName
  type: string
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
schema_file: json-schema/microsoft-graph-identity-user-update-schema.json
slug: microsoft-graph-identity-user-update
source_filename: microsoft-graph-identity-user-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UserUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Properties that can be updated on an existing user.\",\n  \"properties\": {\n    \"accountEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"givenName\": {\n      \"type\": \"string\"\n    },\n    \"surname\": {\n      \"type\": \"string\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\"\n    },\n    \"department\": {\n      \"type\": \"string\"\n    },\n    \"mail\": {\n      \"type\": \"string\"\n    },\n    \"mobilePhone\": {\n      \"type\": \"string\"\n    },\n    \"businessPhones\": {\n      \"type\": \"array\"\n    },\n    \"city\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"country\": {\n      \"type\": \"string\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\"\n    },\n    \"streetAddress\"\
  : {\n      \"type\": \"string\"\n    },\n    \"officeLocation\": {\n      \"type\": \"string\"\n    },\n    \"usageLocation\": {\n      \"type\": \"string\"\n    },\n    \"preferredLanguage\": {\n      \"type\": \"string\"\n    },\n    \"employeeId\": {\n      \"type\": \"string\"\n    },\n    \"employeeType\": {\n      \"type\": \"string\"\n    },\n    \"companyName\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/json-schema/microsoft-graph-identity-user-update-schema.json
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
title: UserUpdate
---
