---
description: ''
layout: schema
name: Element
properties_list:
- description: Element identifier
  name: id
  type: string
- description: Element name
  name: name
  type: string
- description: ArchiMate element type
  name: type
  type: string
- description: Architecture layer
  name: layer
  type: string
- description: Element description
  name: description
  type: string
provider_name: ArchiMate
provider_slug: archimate
schema_file: json-schema/archimate-model-exchange-api-element-schema.json
slug: archimate-model-exchange-api-element
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Element identifier\",\n      \"example\": \"elem-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Element name\",\n      \"example\": \"Customer Portal\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"ArchiMate element type\",\n      \"enum\": [\n        \"ApplicationComponent\",\n        \"ApplicationService\",\n        \"DataObject\",\n        \"BusinessProcess\",\n        \"BusinessRole\",\n        \"BusinessActor\",\n        \"SystemSoftware\",\n        \"Node\",\n        \"NetworkPath\",\n        \"Technology\",\n        \"Artifact\"\n      ],\n      \"example\": \"ApplicationComponent\"\n    },\n    \"layer\": {\n      \"type\": \"string\",\n      \"description\": \"Architecture layer\",\n      \"enum\": [\n        \"Business\",\n        \"Application\",\n        \"Technology\",\n  \
  \      \"Strategy\",\n        \"Motivation\",\n        \"Implementation\",\n        \"Physical\"\n      ],\n      \"example\": \"Application\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Element description\",\n      \"example\": \"Web portal for customer self-service\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-element-schema.json\",\n  \"title\": \"Element\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archimate/refs/heads/main/json-schema/archimate-model-exchange-api-element-schema.json
tags:
- Enterprise Architecture
- Architecture Framework
- Modeling Language
- Business Architecture
- Technology Architecture
- Standard
- Open Group
title: Element
---
