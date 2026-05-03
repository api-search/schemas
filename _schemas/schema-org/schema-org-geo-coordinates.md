---
description: The geographic coordinates of a place or event.
layout: schema
name: Schema.org GeoCoordinates
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The latitude of a location.
  name: latitude
  type: number
- description: The longitude of a location.
  name: longitude
  type: number
- description: The elevation of a location in meters.
  name: elevation
  type: object
- description: Physical address of the location.
  name: address
  type: object
- description: The country. Use the two-letter ISO 3166-1 alpha-2 country code.
  name: addressCountry
  type: string
- description: The postal code.
  name: postalCode
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-geo-coordinates-schema.json
slug: schema-org-geo-coordinates
source_filename: schema-org-geo-coordinates-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/geo-coordinates.json\",\n  \"title\": \"Schema.org GeoCoordinates\",\n  \"description\": \"The geographic coordinates of a place or event.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"latitude\", \"longitude\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"GeoCoordinates\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"The latitude of a location.\",\n      \"minimum\": -90,\n      \"maximum\": 90\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"The longitude of a location.\",\n      \"minimum\": -180,\n      \"maximum\": 180\n    },\n    \"elevation\": {\n      \"oneOf\": [\n        { \"type\"\
  : \"number\" },\n        { \"type\": \"string\" }\n      ],\n      \"description\": \"The elevation of a location in meters.\"\n    },\n    \"address\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"$ref\": \"schema-org-postal-address-schema.json\" }\n      ],\n      \"description\": \"Physical address of the location.\"\n    },\n    \"addressCountry\": {\n      \"type\": \"string\",\n      \"description\": \"The country. Use the two-letter ISO 3166-1 alpha-2 country code.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-geo-coordinates-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org GeoCoordinates
---
