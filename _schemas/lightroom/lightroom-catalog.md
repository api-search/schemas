---
description: Schema for an Adobe Lightroom cloud catalog. Each Lightroom customer has a single catalog that serves as the top-level container for all their assets, albums, and metadata.
layout: schema
name: Lightroom Catalog
properties_list:
- description: Unique identifier for the catalog
  name: id
  type: string
- description: Resource type identifier
  name: type
  type: string
- description: Server-side timestamp when the catalog was created
  name: created
  type: string
- description: Server-side timestamp when the catalog was last updated
  name: updated
  type: string
- description: Catalog metadata payload
  name: payload
  type: object
- description: ''
  name: links
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-catalog-schema.json
slug: lightroom-catalog
source_filename: lightroom-catalog-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://lr.adobe.io/schemas/lightroom/catalog.json\",\n  \"title\": \"Lightroom Catalog\",\n  \"description\": \"Schema for an Adobe Lightroom cloud catalog. Each Lightroom customer has a single catalog that serves as the top-level container for all their assets, albums, and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the catalog\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier\",\n      \"const\": \"catalog\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Server-side timestamp when the catalog was created\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Server-side timestamp when the catalog was last updated\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Catalog metadata payload\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the catalog\"\n        },\n        \"userCreated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"User-side timestamp when the catalog was created\"\n        },\n        \"userUpdated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"User-side timestamp when the catalog was last updated\"\n        }\n      }\n    },\n    \"links\": {\n      \"$ref\": \"#/$defs/Links\"\n    }\n  },\n  \"$defs\": {\n    \"Links\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation links for the catalog resource\",\n      \"properties\": {\n        \"self\": {\n          \"$ref\"\
  : \"#/$defs/Link\"\n        },\n        \"assets\": {\n          \"$ref\": \"#/$defs/Link\"\n        },\n        \"albums\": {\n          \"$ref\": \"#/$defs/Link\"\n        }\n      },\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    },\n    \"Link\": {\n      \"type\": \"object\",\n      \"description\": \"A hyperlink reference to a related resource\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"description\": \"URL of the linked resource\"\n        }\n      },\n      \"required\": [\n        \"href\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-catalog-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: Lightroom Catalog
---
