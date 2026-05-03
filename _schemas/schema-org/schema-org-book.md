---
description: A book.
layout: schema
name: Schema.org Book
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the book.
  name: name
  type: string
- description: A description of the book.
  name: description
  type: string
- description: URL of the book.
  name: url
  type: string
- description: An image of the book.
  name: image
  type: object
- description: The author of this book.
  name: author
  type: object
- description: The publisher of this book.
  name: publisher
  type: object
- description: The ISBN of the book.
  name: isbn
  type: string
- description: The number of pages in the book.
  name: numberOfPages
  type: integer
- description: The edition of the book.
  name: bookEdition
  type: string
- description: The format of the book.
  name: bookFormat
  type: string
- description: The illustrator of the book.
  name: illustrator
  type: object
- description: Date of first publication.
  name: datePublished
  type: string
- description: The language of the book.
  name: inLanguage
  type: string
- description: Genre of the book.
  name: genre
  type: string
- description: An award won by the book.
  name: award
  type: object
- description: The overall rating.
  name: aggregateRating
  type: object
- description: A review of the book.
  name: review
  type: object
- description: An offer to provide this book.
  name: offers
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-book-schema.json
slug: schema-org-book
source_filename: schema-org-book-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/book.json\",\n  \"title\": \"Schema.org Book\",\n  \"description\": \"A book.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"Book\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the book.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the book.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the book.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\"\
  \ }\n      ],\n      \"description\": \"An image of the book.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-person-schema.json\" } }\n      ],\n      \"description\": \"The author of this book.\"\n    },\n    \"publisher\": {\n      \"$ref\": \"schema-org-organization-schema.json\",\n      \"description\": \"The publisher of this book.\"\n    },\n    \"isbn\": {\n      \"type\": \"string\",\n      \"description\": \"The ISBN of the book.\"\n    },\n    \"numberOfPages\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of pages in the book.\"\n    },\n    \"bookEdition\": {\n      \"type\": \"string\",\n      \"description\": \"The edition of the book.\"\n    },\n    \"bookFormat\": {\n      \"type\": \"string\",\n      \"enum\": [\"AudiobookFormat\", \"EBook\", \"GraphicNovel\", \"Hardcover\", \"Paperback\"],\n      \"description\": \"The\
  \ format of the book.\"\n    },\n    \"illustrator\": {\n      \"$ref\": \"schema-org-person-schema.json\",\n      \"description\": \"The illustrator of the book.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"inLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the book.\"\n    },\n    \"genre\": {\n      \"type\": \"string\",\n      \"description\": \"Genre of the book.\"\n    },\n    \"award\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"An award won by the book.\"\n    },\n    \"aggregateRating\": {\n      \"$ref\": \"schema-org-aggregate-rating-schema.json\",\n      \"description\": \"The overall rating.\"\n    },\n    \"review\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-review-schema.json\" },\n    \
  \    { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-review-schema.json\" } }\n      ],\n      \"description\": \"A review of the book.\"\n    },\n    \"offers\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-offer-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-offer-schema.json\" } }\n      ],\n      \"description\": \"An offer to provide this book.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-book-schema.json
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
title: Schema.org Book
---
