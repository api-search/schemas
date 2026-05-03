---
description: A review of an item, such as a product, service, or creative work.
layout: schema
name: Schema.org Review
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the review.
  name: name
  type: string
- description: A description of the review.
  name: description
  type: string
- description: The actual body of the review.
  name: reviewBody
  type: string
- description: The rating given in this review.
  name: reviewRating
  type: object
- description: The author of this review.
  name: author
  type: object
- description: The publisher of this review.
  name: publisher
  type: object
- description: Date of first publication.
  name: datePublished
  type: string
- description: The date the review was most recently modified.
  name: dateModified
  type: string
- description: The item that is being reviewed.
  name: itemReviewed
  type: object
- description: Positive aspects of the reviewed item.
  name: positiveNotes
  type: object
- description: Negative aspects of the reviewed item.
  name: negativeNotes
  type: object
- description: URL of the review.
  name: url
  type: string
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-review-schema.json
slug: schema-org-review
source_filename: schema-org-review-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/review.json\",\n  \"title\": \"Schema.org Review\",\n  \"description\": \"A review of an item, such as a product, service, or creative work.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"Review\", \"ClaimReview\", \"CriticReview\", \"EmployerReview\", \"MediaReview\", \"Recommendation\", \"UserReview\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the review.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the review.\"\n    },\n    \"reviewBody\": {\n      \"type\": \"string\",\n      \"description\": \"The actual body\
  \ of the review.\"\n    },\n    \"reviewRating\": {\n      \"$ref\": \"#/$defs/Rating\",\n      \"description\": \"The rating given in this review.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The author of this review.\"\n    },\n    \"publisher\": {\n      \"$ref\": \"schema-org-organization-schema.json\",\n      \"description\": \"The publisher of this review.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the review was most recently modified.\"\n    },\n    \"itemReviewed\": {\n      \"type\": \"object\",\n      \"description\": \"The item that is being reviewed.\",\n      \"properties\": {\n      \
  \  \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    },\n    \"positiveNotes\": {\n      \"type\": \"object\",\n      \"description\": \"Positive aspects of the reviewed item.\",\n      \"properties\": {\n        \"@type\": { \"const\": \"ItemList\" },\n        \"itemListElement\": { \"type\": \"array\", \"items\": { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"ListItem\" }, \"name\": { \"type\": \"string\" } } } }\n      }\n    },\n    \"negativeNotes\": {\n      \"type\": \"object\",\n      \"description\": \"Negative aspects of the reviewed item.\",\n      \"properties\": {\n        \"@type\": { \"const\": \"ItemList\" },\n        \"itemListElement\": { \"type\": \"array\", \"items\": { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"ListItem\" }, \"name\": { \"type\": \"string\" } } } }\n      }\n    },\n    \"url\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the review.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  },\n  \"$defs\": {\n    \"Rating\": {\n      \"type\": \"object\",\n      \"description\": \"A rating is an evaluation on a numeric scale.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"Rating\" },\n        \"ratingValue\": { \"oneOf\": [{ \"type\": \"number\" }, { \"type\": \"string\" }], \"description\": \"The rating for the content.\" },\n        \"bestRating\": { \"oneOf\": [{ \"type\": \"number\" }, { \"type\": \"string\" }], \"description\": \"The highest value allowed in this rating system.\" },\n        \"worstRating\": { \"oneOf\": [{ \"\
  type\": \"number\" }, { \"type\": \"string\" }], \"description\": \"The lowest value allowed in this rating system.\" },\n        \"ratingExplanation\": { \"type\": \"string\", \"description\": \"A short explanation for the rating.\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-review-schema.json
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
title: Schema.org Review
---
