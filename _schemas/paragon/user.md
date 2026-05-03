---
description: A Connected User represents an end-user of your application who has authenticated and connected third-party integrations through Paragon.
layout: schema
name: Paragon Connected User
properties_list:
- description: The unique identifier for the Connected User.
  name: id
  type: string
- description: Arbitrary key-value metadata associated with the Connected User.
  name: meta
  type: object
- description: Whether the user is currently authenticated with Paragon.
  name: authenticated
  type: boolean
- description: A map of integration types to their status for this user.
  name: integrations
  type: object
provider_name: Paragon
provider_slug: paragon
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/paragon/blob/main/json-schema/user.json\",\n  \"title\": \"Paragon Connected User\",\n  \"description\": \"A Connected User represents an end-user of your application who has authenticated and connected third-party integrations through Paragon.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Connected User.\"\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary key-value metadata associated with the Connected User.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"authenticated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user is currently authenticated with Paragon.\"\n    },\n    \"integrations\": {\n      \"type\": \"object\",\n      \"description\": \"\
  A map of integration types to their status for this user.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/UserIntegration\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"UserIntegration\": {\n      \"type\": \"object\",\n      \"description\": \"The status of a specific integration for a Connected User.\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the integration is enabled for this user.\"\n        },\n        \"credentialStatus\": {\n          \"type\": \"string\",\n          \"description\": \"The status of the integration credential.\",\n          \"enum\": [\"VALID\", \"INVALID\", \"EXPIRED\"]\n        },\n        \"providerId\": {\n          \"type\": \"string\",\n          \"description\": \"The provider-specific user ID.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/paragon/refs/heads/main/json-schema/user.json
tags:
- Embedded iPaaS
- Integrations
title: Paragon Connected User
---
