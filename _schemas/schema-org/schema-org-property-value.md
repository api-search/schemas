---
description: A property-value pair, e.g. representing a feature of a product or place.
layout: schema
name: Schema.org PropertyValue
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the property.
  name: name
  type: string
- description: The value of the property.
  name: value
  type: object
- description: A commonly used identifier for the characteristic represented by the property.
  name: propertyID
  type: string
- description: The unit of measurement given using the UN/CEFACT Common Code.
  name: unitCode
  type: string
- description: A string indicating the unit of measurement.
  name: unitText
  type: string
- description: The lower value of some characteristic or property.
  name: minValue
  type: number
- description: The upper value of some characteristic or property.
  name: maxValue
  type: number
- description: A technique or technology used in a measurement.
  name: measurementTechnique
  type: string
- description: A pointer to a secondary value that provides additional information.
  name: valueReference
  type: object
- description: URL of the property value.
  name: url
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-property-value-schema.json
slug: schema-org-property-value
source_filename: schema-org-property-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/property-value.json\",\n  \"title\": \"Schema.org PropertyValue\",\n  \"description\": \"A property-value pair, e.g. representing a feature of a product or place.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"PropertyValue\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the property.\"\n    },\n    \"value\": {\n      \"description\": \"The value of the property.\"\n    },\n    \"propertyID\": {\n      \"type\": \"string\",\n      \"description\": \"A commonly used identifier for the characteristic represented by the property.\"\n    },\n    \"unitCode\": {\n      \"\
  type\": \"string\",\n      \"description\": \"The unit of measurement given using the UN/CEFACT Common Code.\"\n    },\n    \"unitText\": {\n      \"type\": \"string\",\n      \"description\": \"A string indicating the unit of measurement.\"\n    },\n    \"minValue\": {\n      \"type\": \"number\",\n      \"description\": \"The lower value of some characteristic or property.\"\n    },\n    \"maxValue\": {\n      \"type\": \"number\",\n      \"description\": \"The upper value of some characteristic or property.\"\n    },\n    \"measurementTechnique\": {\n      \"type\": \"string\",\n      \"description\": \"A technique or technology used in a measurement.\"\n    },\n    \"valueReference\": {\n      \"type\": \"object\",\n      \"description\": \"A pointer to a secondary value that provides additional information.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"value\": {}\n      }\n    },\n    \"url\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the property value.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-property-value-schema.json
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
title: Schema.org PropertyValue
---
