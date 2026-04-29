---
description: Schema for a Crossref Work record returned by /works endpoints, capturing the core scholarly metadata fields.
layout: schema
name: Crossref Work
properties_list:
- description: Digital Object Identifier of the work.
  name: DOI
  type: string
- description: Resolvable URL for the DOI.
  name: URL
  type: string
- description: Crossref work type ID such as journal-article, book-chapter, dataset, preprint.
  name: type
  type: string
- description: ''
  name: title
  type: array
- description: ''
  name: subtitle
  type: array
- description: ''
  name: container-title
  type: array
- description: ''
  name: short-container-title
  type: array
- description: ''
  name: publisher
  type: string
- description: ''
  name: publisher-location
  type: string
- description: ''
  name: ISSN
  type: array
- description: ''
  name: ISBN
  type: array
- description: ''
  name: issue
  type: string
- description: ''
  name: volume
  type: string
- description: ''
  name: page
  type: string
- description: ''
  name: article-number
  type: string
- description: ''
  name: abstract
  type: string
- description: ''
  name: subject
  type: array
- description: ''
  name: author
  type: array
- description: ''
  name: editor
  type: array
- description: ''
  name: translator
  type: array
- description: ''
  name: issued
  type: object
- description: ''
  name: published
  type: object
- description: ''
  name: published-print
  type: object
- description: ''
  name: published-online
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: deposited
  type: object
- description: ''
  name: indexed
  type: object
- description: ''
  name: reference-count
  type: integer
- description: ''
  name: references-count
  type: integer
- description: ''
  name: is-referenced-by-count
  type: integer
- description: ''
  name: score
  type: number
- description: ''
  name: member
  type: string
- description: ''
  name: prefix
  type: string
- description: ''
  name: license
  type: array
- description: ''
  name: funder
  type: array
- description: ''
  name: link
  type: array
- description: ''
  name: reference
  type: array
- description: ''
  name: relation
  type: object
provider_name: Crossref
provider_slug: crossref
schema_file: json-schema/crossref-work-schema.json
slug: crossref-work
source_filename: crossref-work-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/crossref/json-schema/crossref-work-schema.json\",\n  \"title\": \"Crossref Work\",\n  \"description\": \"Schema for a Crossref Work record returned by /works endpoints, capturing the core scholarly metadata fields.\",\n  \"type\": \"object\",\n  \"required\": [\"DOI\", \"type\"],\n  \"properties\": {\n    \"DOI\": {\n      \"type\": \"string\",\n      \"description\": \"Digital Object Identifier of the work.\",\n      \"pattern\": \"^10\\\\.\"\n    },\n    \"URL\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Resolvable URL for the DOI.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Crossref work type ID such as journal-article, book-chapter, dataset, preprint.\"\n    },\n    \"title\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"subtitle\": {\n\
  \      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"container-title\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"short-container-title\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"publisher\": { \"type\": \"string\" },\n    \"publisher-location\": { \"type\": \"string\" },\n    \"ISSN\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"ISBN\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"issue\": { \"type\": \"string\" },\n    \"volume\": { \"type\": \"string\" },\n    \"page\": { \"type\": \"string\" },\n    \"article-number\": { \"type\": \"string\" },\n    \"abstract\": { \"type\": \"string\" },\n    \"subject\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" }\n    },\n    \"author\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Contributor\"\
  \ }\n    },\n    \"editor\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Contributor\" }\n    },\n    \"translator\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Contributor\" }\n    },\n    \"issued\": { \"$ref\": \"#/$defs/PartialDate\" },\n    \"published\": { \"$ref\": \"#/$defs/PartialDate\" },\n    \"published-print\": { \"$ref\": \"#/$defs/PartialDate\" },\n    \"published-online\": { \"$ref\": \"#/$defs/PartialDate\" },\n    \"created\": { \"$ref\": \"#/$defs/Timestamp\" },\n    \"deposited\": { \"$ref\": \"#/$defs/Timestamp\" },\n    \"indexed\": { \"$ref\": \"#/$defs/Timestamp\" },\n    \"reference-count\": { \"type\": \"integer\" },\n    \"references-count\": { \"type\": \"integer\" },\n    \"is-referenced-by-count\": { \"type\": \"integer\" },\n    \"score\": { \"type\": \"number\" },\n    \"member\": { \"type\": \"string\" },\n    \"prefix\": { \"type\": \"string\" },\n    \"license\": {\n      \"type\": \"array\",\n    \
  \  \"items\": { \"$ref\": \"#/$defs/License\" }\n    },\n    \"funder\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Funder\" }\n    },\n    \"link\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/ResourceLink\" }\n    },\n    \"reference\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Reference\" }\n    },\n    \"relation\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    }\n  },\n  \"$defs\": {\n    \"Contributor\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"given\": { \"type\": \"string\" },\n        \"family\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"ORCID\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"authenticated-orcid\": { \"type\": \"boolean\" },\n        \"affiliation\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n   \
  \           \"name\": { \"type\": \"string\" },\n              \"id\": {\n                \"type\": \"array\",\n                \"items\": { \"type\": \"object\" }\n              }\n            }\n          }\n        },\n        \"sequence\": {\n          \"type\": \"string\",\n          \"enum\": [\"first\", \"additional\"]\n        }\n      }\n    },\n    \"PartialDate\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"date-parts\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"integer\" },\n            \"minItems\": 1,\n            \"maxItems\": 3\n          }\n        },\n        \"date-time\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"timestamp\": { \"type\": \"integer\" }\n      }\n    },\n    \"Timestamp\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"date-parts\": {\n          \"type\": \"array\",\n          \"items\": {\n         \
  \   \"type\": \"array\",\n            \"items\": { \"type\": \"integer\" }\n          }\n        },\n        \"date-time\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"timestamp\": { \"type\": \"integer\" }\n      }\n    },\n    \"License\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"URL\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"start\": { \"$ref\": \"#/$defs/PartialDate\" },\n        \"delay-in-days\": { \"type\": \"integer\" },\n        \"content-version\": { \"type\": \"string\" }\n      }\n    },\n    \"Funder\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"DOI\": { \"type\": \"string\" },\n        \"doi-asserted-by\": { \"type\": \"string\" },\n        \"award\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"ResourceLink\": {\n      \"type\": \"object\",\n      \"properties\": {\n   \
  \     \"URL\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"content-type\": { \"type\": \"string\" },\n        \"content-version\": { \"type\": \"string\" },\n        \"intended-application\": { \"type\": \"string\" }\n      }\n    },\n    \"Reference\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"key\": { \"type\": \"string\" },\n        \"DOI\": { \"type\": \"string\" },\n        \"doi-asserted-by\": { \"type\": \"string\" },\n        \"article-title\": { \"type\": \"string\" },\n        \"journal-title\": { \"type\": \"string\" },\n        \"volume\": { \"type\": \"string\" },\n        \"first-page\": { \"type\": \"string\" },\n        \"year\": { \"type\": \"string\" },\n        \"author\": { \"type\": \"string\" },\n        \"unstructured\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/crossref/refs/heads/main/json-schema/crossref-work-schema.json
tags:
- Citations
- DOI
- Funders
- Identifiers
- Journals
- Licenses
- Members
- Metadata
- Open Access
- ORCID
- Prefixes
- Publishers
- Reference Linking
- ROR
- Scholarly
title: Crossref Work
---
