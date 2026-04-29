---
description: JSON:API resource identifier
layout: schema
name: ResourceIdentifier
properties_list:
- description: Resource identifier
  name: id
  type: string
- description: Resource type name
  name: type
  type: string
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-resource-identifier-schema.json
slug: prime-api-resource-identifier
source_filename: prime-api-resource-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-resource-identifier-schema.json\",\n  \"title\": \"ResourceIdentifier\",\n  \"description\": \"JSON:API resource identifier\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Resource identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-resource-identifier-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: ResourceIdentifier
---
