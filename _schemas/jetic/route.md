---
description: A Route defines an Apache Camel integration flow with a source component, one or more destination components, and optional enterprise integration pattern processors.
layout: schema
name: Jetic Route
properties_list:
- description: Unique route identifier.
  name: id
  type: string
- description: Name of the route.
  name: name
  type: string
- description: Source Camel component URI.
  name: from
  type: string
- description: Destination Camel component URIs.
  name: to
  type: array
- description: Enterprise integration pattern processors applied to the route.
  name: processors
  type: array
provider_name: Jetic
provider_slug: jetic
schema_file: json-schema/route.json
slug: route
source_filename: route.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/jetic/blob/main/json-schema/route.json\",\n  \"title\": \"Jetic Route\",\n  \"description\": \"A Route defines an Apache Camel integration flow with a source component, one or more destination components, and optional enterprise integration pattern processors.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique route identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the route.\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"Source Camel component URI.\"\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Destination Camel component URIs.\"\n    },\n    \"processors\": {\n      \"type\": \"array\",\n      \"items\": {\n\
  \        \"type\": \"string\"\n      },\n      \"description\": \"Enterprise integration pattern processors applied to the route.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/json-schema/route.json
tags:
- Apache Camel
- Integrations
- iPaaS
- Pro-Code API Composition
title: Jetic Route
---
