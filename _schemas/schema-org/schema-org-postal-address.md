---
description: The mailing address.
layout: schema
name: Schema.org PostalAddress
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The street address.
  name: streetAddress
  type: string
- description: The locality (city).
  name: addressLocality
  type: string
- description: The region (state, province).
  name: addressRegion
  type: string
- description: The postal code.
  name: postalCode
  type: string
- description: The country. Use the two-letter ISO 3166-1 alpha-2 country code.
  name: addressCountry
  type: string
- description: The post office box number.
  name: postOfficeBoxNumber
  type: string
- description: The name of the address.
  name: name
  type: string
- description: The telephone number.
  name: telephone
  type: string
- description: The fax number.
  name: faxNumber
  type: string
- description: Email address.
  name: email
  type: string
- description: A person or organization can have different contact points for different purposes.
  name: contactType
  type: string
- description: The geographic area where a service is provided.
  name: areaServed
  type: string
- description: A language someone may use with or at the item.
  name: availableLanguage
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-postal-address-schema.json
slug: schema-org-postal-address
source_filename: schema-org-postal-address-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/postal-address.json\",\n  \"title\": \"Schema.org PostalAddress\",\n  \"description\": \"The mailing address.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"PostalAddress\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"streetAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The street address.\"\n    },\n    \"addressLocality\": {\n      \"type\": \"string\",\n      \"description\": \"The locality (city).\"\n    },\n    \"addressRegion\": {\n      \"type\": \"string\",\n      \"description\": \"The region (state, province).\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code.\"\n   \
  \ },\n    \"addressCountry\": {\n      \"type\": \"string\",\n      \"description\": \"The country. Use the two-letter ISO 3166-1 alpha-2 country code.\"\n    },\n    \"postOfficeBoxNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The post office box number.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the address.\"\n    },\n    \"telephone\": {\n      \"type\": \"string\",\n      \"description\": \"The telephone number.\"\n    },\n    \"faxNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The fax number.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address.\"\n    },\n    \"contactType\": {\n      \"type\": \"string\",\n      \"description\": \"A person or organization can have different contact points for different purposes.\"\n    },\n    \"areaServed\": {\n      \"type\": \"string\",\n      \"description\": \"The geographic area\
  \ where a service is provided.\"\n    },\n    \"availableLanguage\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"A language someone may use with or at the item.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-postal-address-schema.json
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
title: Schema.org PostalAddress
---
