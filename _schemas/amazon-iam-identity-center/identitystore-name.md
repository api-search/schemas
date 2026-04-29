---
description: The full name of the user.
layout: schema
name: Name
properties_list:
- description: ''
  name: Formatted
  type: object
- description: ''
  name: FamilyName
  type: object
- description: ''
  name: GivenName
  type: object
- description: ''
  name: MiddleName
  type: object
- description: ''
  name: HonorificPrefix
  type: object
- description: ''
  name: HonorificSuffix
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-name-schema.json
slug: identitystore-name
source_filename: identitystore-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-name-schema.json\",\n  \"title\": \"Name\",\n  \"description\": \"The full name of the user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Formatted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing a formatted version of the name for display.\"\n        }\n      ]\n    },\n    \"FamilyName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"The family name of the user.\"\n        }\n      ]\n    },\n    \"GivenName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n   \
  \       \"description\": \"The given name of the user.\"\n        }\n      ]\n    },\n    \"MiddleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"The middle name of the user.\"\n        }\n      ]\n    },\n    \"HonorificPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"The honorific prefix of the user. For example, \\\"Dr.\\\"\"\n        }\n      ]\n    },\n    \"HonorificSuffix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"The honorific suffix of the user. For example, \\\"M.D.\\\"\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-name-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: Name
---
