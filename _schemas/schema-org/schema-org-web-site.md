---
description: A WebSite is a set of related web pages and other items typically served from a single web domain and accessible via URLs.
layout: schema
name: Schema.org WebSite
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the website.
  name: name
  type: string
- description: A description of the website.
  name: description
  type: string
- description: URL of the website.
  name: url
  type: string
- description: Indicates a potential Action, typically a SearchAction for site search.
  name: potentialAction
  type: object
- description: The publisher of the website.
  name: publisher
  type: object
- description: The language(s) of the website content.
  name: inLanguage
  type: object
- description: An alias for the website.
  name: alternateName
  type: string
- description: An image of the website.
  name: image
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-web-site-schema.json
slug: schema-org-web-site
source_filename: schema-org-web-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/web-site.json\",\n  \"title\": \"Schema.org WebSite\",\n  \"description\": \"A WebSite is a set of related web pages and other items typically served from a single web domain and accessible via URLs.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\", \"url\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"WebSite\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the website.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the website.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the website.\"\
  \n    },\n    \"potentialAction\": {\n      \"$ref\": \"schema-org-search-action-schema.json\",\n      \"description\": \"Indicates a potential Action, typically a SearchAction for site search.\"\n    },\n    \"publisher\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The publisher of the website.\"\n    },\n    \"inLanguage\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"The language(s) of the website content.\"\n    },\n    \"alternateName\": {\n      \"type\": \"string\",\n      \"description\": \"An alias for the website.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the\
  \ website.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-web-site-schema.json
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
title: Schema.org WebSite
---
