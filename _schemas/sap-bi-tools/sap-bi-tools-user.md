---
description: A user record conforming to SCIM 2.0 protocol for SAP Analytics Cloud. Contains user profile attributes, roles, and team memberships.
layout: schema
name: SAP Analytics Cloud User
properties_list:
- description: The unique identifier assigned to the user
  name: id
  type: string
- description: The login username for the user
  name: userName
  type: string
- description: The user's name components
  name: name
  type: object
- description: The display name of the user
  name: displayName
  type: string
- description: Email addresses for the user
  name: emails
  type: array
- description: Whether the user account is active
  name: active
  type: boolean
- description: Roles assigned to the user
  name: roles
  type: array
- description: Teams the user belongs to
  name: groups
  type: array
provider_name: SAP BI Tools
provider_slug: sap-bi-tools
schema_file: json-schema/sap-bi-tools-user-schema.json
slug: sap-bi-tools-user
source_filename: sap-bi-tools-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sap-bi-tools/json-schema/sap-bi-tools-user-schema.json\",\n  \"title\": \"SAP Analytics Cloud User\",\n  \"description\": \"A user record conforming to SCIM 2.0 protocol for SAP Analytics Cloud. Contains user profile attributes, roles, and team memberships.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier assigned to the user\"\n    },\n    \"userName\": {\n      \"type\": \"string\",\n      \"description\": \"The login username for the user\"\n    },\n    \"name\": {\n      \"type\": \"object\",\n      \"description\": \"The user's name components\",\n      \"properties\": {\n        \"givenName\": {\n          \"type\": \"string\",\n          \"description\": \"The first name of the user\"\n        },\n        \"familyName\": {\n          \"type\": \"string\",\n      \
  \    \"description\": \"The last name of the user\"\n        },\n        \"formatted\": {\n          \"type\": \"string\",\n          \"description\": \"The full formatted name of the user\"\n        }\n      }\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the user\"\n    },\n    \"emails\": {\n      \"type\": \"array\",\n      \"description\": \"Email addresses for the user\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"format\": \"email\",\n            \"description\": \"The email address\"\n          },\n          \"primary\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether this is the primary email\"\n          }\n        }\n      }\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user account is active\"\n    },\n    \"roles\": {\n      \"\
  type\": \"array\",\n      \"description\": \"Roles assigned to the user\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The role identifier\"\n          }\n        }\n      }\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"Teams the user belongs to\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The team identifier\"\n          },\n          \"display\": {\n            \"type\": \"string\",\n            \"description\": \"The team display name\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"userName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/json-schema/sap-bi-tools-user-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
title: SAP Analytics Cloud User
---
