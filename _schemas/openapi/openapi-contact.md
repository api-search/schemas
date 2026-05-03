---
description: Contact information for the exposed API.
layout: schema
name: OpenAPI Contact Object
properties_list:
- description: The identifying name of the contact person or organization.
  name: name
  type: string
- description: The URL pointing to the contact information.
  name: url
  type: string
- description: The email address of the contact person or organization.
  name: email
  type: string
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-contact.json
slug: openapi-contact
source_filename: openapi-contact.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-contact.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Contact Object\",\n  \"description\": \"Contact information for the exposed API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The identifying name of the contact person or organization.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL pointing to the contact information.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the contact person or organization.\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-contact.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Contact Object
---
