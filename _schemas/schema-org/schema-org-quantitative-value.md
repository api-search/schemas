---
description: A point value or interval for product characteristics and other purposes.
layout: schema
name: Schema.org QuantitativeValue
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The value.
  name: value
  type: number
- description: The lower value of some characteristic or property.
  name: minValue
  type: number
- description: The upper value of some characteristic or property.
  name: maxValue
  type: number
- description: The unit of measurement given using the UN/CEFACT Common Code.
  name: unitCode
  type: string
- description: A string indicating the unit of measurement.
  name: unitText
  type: string
- description: The name of the quantity.
  name: name
  type: string
- description: A property-value pair representing an additional characteristic.
  name: additionalProperty
  type: object
- description: A pointer to a secondary value that provides additional information.
  name: valueReference
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-quantitative-value-schema.json
slug: schema-org-quantitative-value
source_filename: schema-org-quantitative-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/quantitative-value.json\",\n  \"title\": \"Schema.org QuantitativeValue\",\n  \"description\": \"A point value or interval for product characteristics and other purposes.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"QuantitativeValue\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"The value.\"\n    },\n    \"minValue\": {\n      \"type\": \"number\",\n      \"description\": \"The lower value of some characteristic or property.\"\n    },\n    \"maxValue\": {\n      \"type\": \"number\",\n      \"description\": \"The upper value of some characteristic or property.\"\n    },\n    \"unitCode\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The unit of measurement given using the UN/CEFACT Common Code.\"\n    },\n    \"unitText\": {\n      \"type\": \"string\",\n      \"description\": \"A string indicating the unit of measurement.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the quantity.\"\n    },\n    \"additionalProperty\": {\n      \"$ref\": \"schema-org-property-value-schema.json\",\n      \"description\": \"A property-value pair representing an additional characteristic.\"\n    },\n    \"valueReference\": {\n      \"type\": \"object\",\n      \"description\": \"A pointer to a secondary value that provides additional information.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"value\": {}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-quantitative-value-schema.json
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
title: Schema.org QuantitativeValue
---
