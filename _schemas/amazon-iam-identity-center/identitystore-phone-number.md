---
description: The phone number associated with the user.
layout: schema
name: PhoneNumber
properties_list:
- description: ''
  name: Value
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Primary
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-phone-number-schema.json
slug: identitystore-phone-number
source_filename: identitystore-phone-number-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-phone-number-schema.json\",\n  \"title\": \"PhoneNumber\",\n  \"description\": \"The phone number associated with the user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing a phone number. For example, \\\"8675309\\\" or \\\"+1 (800) 123-4567\\\".\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string representing the type of a phone number. For example, \\\"Mobile.\\\"\"\n        }\n      ]\n    },\n    \"Primary\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/SensitiveBooleanType\"\n        },\n        {\n          \"description\": \"A Boolean value representing whether this is the primary phone number for the associated resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-phone-number-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: PhoneNumber
---
