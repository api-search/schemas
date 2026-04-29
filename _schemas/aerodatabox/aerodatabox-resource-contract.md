---
description: Single media resource data
layout: schema
name: ResourceContract
properties_list:
- description: URL of the resource
  name: url
  type: string
- description: URL of web-page containing the resource
  name: webUrl
  type: string
- description: Author name of the resource
  name: author
  type: string
- description: Title of the resource
  name: title
  type: string
- description: Description of the resource
  name: description
  type: string
- description: ''
  name: license
  type: object
- description: Attributions maintaining copyright, ownership and other legal information adjusted for displaying as HTML. Each element represent one line.
  name: htmlAttributions
  type: array
provider_name: AeroDataBox
provider_slug: aerodatabox
schema_file: json-schema/aerodatabox-resource-contract-schema.json
slug: aerodatabox-resource-contract
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-resource-contract-schema.json\",\n  \"title\": \"ResourceContract\",\n  \"description\": \"Single media resource data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"minLength\": 1,\n      \"type\": \"string\",\n      \"description\": \"URL of the resource\"\n    },\n    \"webUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL of web-page containing the resource\",\n      \"nullable\": true\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Author name of the resource\",\n      \"nullable\": true\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the resource\",\n      \"nullable\": true\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description\
  \ of the resource\",\n      \"nullable\": true\n    },\n    \"license\": {\n      \"$ref\": \"#/components/schemas/LicenseType\"\n    },\n    \"htmlAttributions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Attributions maintaining copyright, ownership and other legal information adjusted for displaying\\r\\nas HTML. Each element represent one line.\",\n      \"nullable\": true\n    }\n  },\n  \"required\": [\n    \"license\",\n    \"url\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aerodatabox/refs/heads/main/json-schema/aerodatabox-resource-contract-schema.json
tags:
- Aviation
- Flights
- Aerospace
- Flight Data
- Airport Data
title: ResourceContract
---
