---
description: Metadata assigned to a directory consisting of a key-value pair.
layout: schema
name: Tag
properties_list:
- description: ''
  name: Key
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-tag-schema.json
slug: amazon-directory-service-tag
source_filename: amazon-directory-service-tag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-tag-schema.json\",\n  \"title\": \"Tag\",\n  \"description\": \"Metadata assigned to a directory consisting of a key-value pair.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKey\"\n        },\n        {\n          \"description\": \"Required name of the tag. The string value can be Unicode characters and cannot be prefixed with \\\"aws:\\\". The string can contain only the set of Unicode letters, digits, white-space, '_', '.', '/', '=', '+', '-' (Java regex: \\\"^([\\\\\\\\p{L}\\\\\\\\p{Z}\\\\\\\\p{N}_.:/=+\\\\\\\\-]*)$\\\").\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagValue\"\n        },\n \
  \       {\n          \"description\": \"The optional value of the tag. The string value can be Unicode characters. The string can contain only the set of Unicode letters, digits, white-space, '_', '.', '/', '=', '+', '-' (Java regex: \\\"^([\\\\\\\\p{L}\\\\\\\\p{Z}\\\\\\\\p{N}_.:/=+\\\\\\\\-]*)$\\\").\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Key\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-tag-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: Tag
---
