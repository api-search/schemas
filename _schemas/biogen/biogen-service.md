---
description: An available Biogen API service.
layout: schema
name: Service
properties_list:
- description: Service identifier.
  name: id
  type: string
- description: Service name.
  name: name
  type: string
- description: Service description.
  name: description
  type: string
- description: Service availability status.
  name: status
  type: string
provider_name: Biogen
provider_slug: biogen
schema_file: json-schema/biogen-service-schema.json
slug: biogen-service
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Service\",\n  \"type\": \"object\",\n  \"description\": \"An available Biogen API service.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Service identifier.\",\n      \"example\": \"ccs-crx\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Service name.\",\n      \"example\": \"CCS-CRX API\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Service description.\",\n      \"example\": \"Copaxone CRX API service\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Service availability status.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"maintenance\"\n      ],\n      \"example\": \"active\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/json-schema/biogen-service-schema.json
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
title: Service
---
