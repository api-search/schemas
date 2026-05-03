---
description: The average rating based on multiple ratings or reviews.
layout: schema
name: Schema.org AggregateRating
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The rating for the content.
  name: ratingValue
  type: object
- description: The highest value allowed in this rating system.
  name: bestRating
  type: object
- description: The lowest value allowed in this rating system.
  name: worstRating
  type: object
- description: The count of total number of ratings.
  name: ratingCount
  type: integer
- description: The count of total number of reviews.
  name: reviewCount
  type: integer
- description: The item that is being rated.
  name: itemReviewed
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-aggregate-rating-schema.json
slug: schema-org-aggregate-rating
source_filename: schema-org-aggregate-rating-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/aggregate-rating.json\",\n  \"title\": \"Schema.org AggregateRating\",\n  \"description\": \"The average rating based on multiple ratings or reviews.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"ratingValue\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"AggregateRating\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"ratingValue\": {\n      \"oneOf\": [\n        { \"type\": \"number\" },\n        { \"type\": \"string\" }\n      ],\n      \"description\": \"The rating for the content.\"\n    },\n    \"bestRating\": {\n      \"oneOf\": [\n        { \"type\": \"number\" },\n        { \"type\": \"string\" }\n      ],\n      \"description\": \"The highest value allowed in this rating system.\"\n \
  \   },\n    \"worstRating\": {\n      \"oneOf\": [\n        { \"type\": \"number\" },\n        { \"type\": \"string\" }\n      ],\n      \"description\": \"The lowest value allowed in this rating system.\"\n    },\n    \"ratingCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The count of total number of ratings.\"\n    },\n    \"reviewCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The count of total number of reviews.\"\n    },\n    \"itemReviewed\": {\n      \"type\": \"object\",\n      \"description\": \"The item that is being rated.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-aggregate-rating-schema.json
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
title: Schema.org AggregateRating
---
