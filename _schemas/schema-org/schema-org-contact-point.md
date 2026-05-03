---
description: A contact point, for example a customer service contact point.
layout: schema
name: Schema.org ContactPoint
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: A person or organization can have different contact points for different purposes (e.g., sales, technical support, billing).
  name: contactType
  type: string
- description: The telephone number.
  name: telephone
  type: string
- description: Email address.
  name: email
  type: string
- description: The fax number.
  name: faxNumber
  type: string
- description: URL of the contact point.
  name: url
  type: string
- description: The geographic area where a service is provided.
  name: areaServed
  type: string
- description: A language someone may use with or at the item.
  name: availableLanguage
  type: object
- description: An option available on this contact point.
  name: contactOption
  type: string
- description: The hours during which this service is available.
  name: hoursAvailable
  type: object
- description: The product or service this support contact point is related to.
  name: productSupported
  type: string
- description: The geographic area where the service is provided.
  name: serviceArea
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-contact-point-schema.json
slug: schema-org-contact-point
source_filename: schema-org-contact-point-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/contact-point.json\",\n  \"title\": \"Schema.org ContactPoint\",\n  \"description\": \"A contact point, for example a customer service contact point.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"ContactPoint\", \"PostalAddress\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"contactType\": {\n      \"type\": \"string\",\n      \"description\": \"A person or organization can have different contact points for different purposes (e.g., sales, technical support, billing).\"\n    },\n    \"telephone\": {\n      \"type\": \"string\",\n      \"description\": \"The telephone number.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\":\
  \ \"email\",\n      \"description\": \"Email address.\"\n    },\n    \"faxNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The fax number.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the contact point.\"\n    },\n    \"areaServed\": {\n      \"type\": \"string\",\n      \"description\": \"The geographic area where a service is provided.\"\n    },\n    \"availableLanguage\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"A language someone may use with or at the item.\"\n    },\n    \"contactOption\": {\n      \"type\": \"string\",\n      \"enum\": [\"HearingImpairedSupported\", \"TollFree\"],\n      \"description\": \"An option available on this contact point.\"\n    },\n    \"hoursAvailable\": {\n      \"type\": \"object\",\n      \"description\": \"The hours during which this service\
  \ is available.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"OpeningHoursSpecification\" },\n        \"dayOfWeek\": { \"type\": \"string\" },\n        \"opens\": { \"type\": \"string\" },\n        \"closes\": { \"type\": \"string\" }\n      }\n    },\n    \"productSupported\": {\n      \"type\": \"string\",\n      \"description\": \"The product or service this support contact point is related to.\"\n    },\n    \"serviceArea\": {\n      \"type\": \"string\",\n      \"description\": \"The geographic area where the service is provided.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-contact-point-schema.json
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
title: Schema.org ContactPoint
---
