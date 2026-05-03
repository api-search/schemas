---
description: 'Any offered product or service. For example: a pair of shoes, a concert ticket, a car, etc.'
layout: schema
name: Schema.org Product
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: The JSON-LD context URL.
  name: '@context'
  type: string
- description: The name of the product.
  name: name
  type: string
- description: A description of the product.
  name: description
  type: string
- description: URL of the product.
  name: url
  type: string
- description: An image of the product.
  name: image
  type: object
- description: The Stock Keeping Unit (SKU) of the product.
  name: sku
  type: string
- description: A Global Trade Item Number (GTIN).
  name: gtin
  type: string
- description: The GTIN-12 code of the product (UPC-A).
  name: gtin12
  type: string
- description: The GTIN-13 code of the product (EAN).
  name: gtin13
  type: string
- description: The GTIN-14 code of the product.
  name: gtin14
  type: string
- description: The GTIN-8 code of the product.
  name: gtin8
  type: string
- description: The Manufacturer Part Number (MPN) of the product.
  name: mpn
  type: string
- description: The brand of the product.
  name: brand
  type: object
- description: The manufacturer of the product.
  name: manufacturer
  type: object
- description: The model of the product.
  name: model
  type: object
- description: A category for the product.
  name: category
  type: object
- description: The color of the product.
  name: color
  type: string
- description: The material the product is made from.
  name: material
  type: string
- description: The weight of the product.
  name: weight
  type: object
- description: The width of the product.
  name: width
  type: object
- description: The height of the product.
  name: height
  type: object
- description: The depth of the product.
  name: depth
  type: object
- description: An offer to provide this product.
  name: offers
  type: object
- description: A review of the product.
  name: review
  type: object
- description: The overall rating.
  name: aggregateRating
  type: object
- description: A pointer to another, somehow related product.
  name: isRelatedTo
  type: object
- description: A pointer to another, functionally similar product.
  name: isSimilarTo
  type: object
- description: A property-value pair representing an additional characteristic.
  name: additionalProperty
  type: object
- description: An award won by or for this product.
  name: award
  type: string
- description: The country of origin of the product.
  name: countryOfOrigin
  type: string
- description: The release date of a product.
  name: releaseDate
  type: string
- description: The date of production of the product.
  name: productionDate
  type: string
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
- description: The identifier property represents any kind of identifier.
  name: identifier
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-product-schema.json
slug: schema-org-product
source_filename: schema-org-product-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/product.json\",\n  \"title\": \"Schema.org Product\",\n  \"description\": \"Any offered product or service. For example: a pair of shoes, a concert ticket, a car, etc.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"Product\", \"IndividualProduct\", \"ProductGroup\", \"ProductModel\", \"Vehicle\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON-LD context URL.\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the product.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the product.\"\n    },\n    \"url\": {\n      \"type\":\
  \ \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the product.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the product.\"\n    },\n    \"sku\": {\n      \"type\": \"string\",\n      \"description\": \"The Stock Keeping Unit (SKU) of the product.\"\n    },\n    \"gtin\": {\n      \"type\": \"string\",\n      \"description\": \"A Global Trade Item Number (GTIN).\"\n    },\n    \"gtin12\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{12}$\",\n      \"description\": \"The GTIN-12 code of the product (UPC-A).\"\n    },\n    \"gtin13\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{13}$\",\n      \"description\": \"The GTIN-13 code of the product (EAN).\"\n    },\n    \"gtin14\":\
  \ {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{14}$\",\n      \"description\": \"The GTIN-14 code of the product.\"\n    },\n    \"gtin8\": {\n      \"type\": \"string\",\n      \"pattern\": \"^\\\\d{8}$\",\n      \"description\": \"The GTIN-8 code of the product.\"\n    },\n    \"mpn\": {\n      \"type\": \"string\",\n      \"description\": \"The Manufacturer Part Number (MPN) of the product.\"\n    },\n    \"brand\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" },\n        { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"Brand\" }, \"name\": { \"type\": \"string\" } } }\n      ],\n      \"description\": \"The brand of the product.\"\n    },\n    \"manufacturer\": {\n      \"$ref\": \"schema-org-organization-schema.json\",\n      \"description\": \"The manufacturer of the product.\"\n    },\n    \"model\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\"\
  : \"object\", \"properties\": { \"@type\": { \"const\": \"ProductModel\" }, \"name\": { \"type\": \"string\" } } }\n      ],\n      \"description\": \"The model of the product.\"\n    },\n    \"category\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"string\", \"format\": \"uri\" }\n      ],\n      \"description\": \"A category for the product.\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"The color of the product.\"\n    },\n    \"material\": {\n      \"type\": \"string\",\n      \"description\": \"The material the product is made from.\"\n    },\n    \"weight\": {\n      \"type\": \"object\",\n      \"description\": \"The weight of the product.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"QuantitativeValue\" },\n        \"value\": { \"type\": \"number\", \"description\": \"The value.\" },\n        \"unitCode\": { \"type\": \"string\", \"description\": \"The unit of measurement\
  \ (UN/CEFACT).\" },\n        \"unitText\": { \"type\": \"string\", \"description\": \"The unit of measurement as text.\" }\n      }\n    },\n    \"width\": {\n      \"type\": \"object\",\n      \"description\": \"The width of the product.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"QuantitativeValue\" },\n        \"value\": { \"type\": \"number\" },\n        \"unitCode\": { \"type\": \"string\" },\n        \"unitText\": { \"type\": \"string\" }\n      }\n    },\n    \"height\": {\n      \"type\": \"object\",\n      \"description\": \"The height of the product.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"QuantitativeValue\" },\n        \"value\": { \"type\": \"number\" },\n        \"unitCode\": { \"type\": \"string\" },\n        \"unitText\": { \"type\": \"string\" }\n      }\n    },\n    \"depth\": {\n      \"type\": \"object\",\n      \"description\": \"The depth of the product.\",\n      \"properties\"\
  : {\n        \"@type\": { \"type\": \"string\", \"const\": \"QuantitativeValue\" },\n        \"value\": { \"type\": \"number\" },\n        \"unitCode\": { \"type\": \"string\" },\n        \"unitText\": { \"type\": \"string\" }\n      }\n    },\n    \"offers\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-offer-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-offer-schema.json\" } }\n      ],\n      \"description\": \"An offer to provide this product.\"\n    },\n    \"review\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-review-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-review-schema.json\" } }\n      ],\n      \"description\": \"A review of the product.\"\n    },\n    \"aggregateRating\": {\n      \"$ref\": \"schema-org-aggregate-rating-schema.json\",\n      \"description\": \"The overall rating.\"\n    },\n    \"isRelatedTo\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n     \
  \   { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"A pointer to another, somehow related product.\"\n    },\n    \"isSimilarTo\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"A pointer to another, functionally similar product.\"\n    },\n    \"additionalProperty\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-property-value-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-property-value-schema.json\" } }\n      ],\n      \"description\": \"A property-value pair representing an additional characteristic.\"\n    },\n    \"award\": {\n      \"type\": \"string\",\n      \"description\": \"An award won by or for this product.\"\n    },\n    \"countryOfOrigin\": {\n      \"type\": \"string\",\n      \"description\": \"The country of origin of the product.\"\n    },\n    \"releaseDate\": {\n    \
  \  \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The release date of a product.\"\n    },\n    \"productionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of production of the product.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier property represents any kind of identifier.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-product-schema.json
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
title: Schema.org Product
---
