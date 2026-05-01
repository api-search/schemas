---
description: Information about an email address.
layout: schema
name: EmailAddress
properties_list:
- description: ''
  name: email
  type: object
- description: ''
  name: verified
  type: object
provider_name: Amazon CodeCatalyst
provider_slug: amazon-codecatalyst
schema_file: json-schema/amazon-codecatalyst-email-address-schema.json
slug: amazon-codecatalyst-email-address
source_filename: amazon-codecatalyst-email-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-email-address-schema.json\",\n  \"title\": \"EmailAddress\",\n  \"description\": \"Information about an email address.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The email address.\"\n        }\n      ]\n    },\n    \"verified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Whether the email address has been verified.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codecatalyst/refs/heads/main/json-schema/amazon-codecatalyst-email-address-schema.json
tags:
- Amazon
- Developer Tools
- CI/CD
- Collaboration
- DevOps
- Source Control
title: EmailAddress
---
