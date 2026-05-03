---
description: A FAQPage is a WebPage presenting one or more Frequently asked questions.
layout: schema
name: Schema.org FAQPage
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the FAQ page.
  name: name
  type: string
- description: A description of the FAQ page.
  name: description
  type: string
- description: URL of the FAQ page.
  name: url
  type: string
- description: The list of questions and answers.
  name: mainEntity
  type: array
- description: Date of first publication.
  name: datePublished
  type: string
- description: The date the FAQ page was most recently modified.
  name: dateModified
  type: string
- description: The author of this FAQ page.
  name: author
  type: object
- description: The publisher of this FAQ page.
  name: publisher
  type: object
- description: The language of the content.
  name: inLanguage
  type: string
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-faq-page-schema.json
slug: schema-org-faq-page
source_filename: schema-org-faq-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/faq-page.json\",\n  \"title\": \"Schema.org FAQPage\",\n  \"description\": \"A FAQPage is a WebPage presenting one or more Frequently asked questions.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"mainEntity\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"FAQPage\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the FAQ page.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the FAQ page.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the FAQ page.\"\n    },\n    \"mainEntity\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"The list of questions and answers.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Question\"\n      }\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date the FAQ page was most recently modified.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The author of this FAQ page.\"\n    },\n    \"publisher\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The publisher of this FAQ page.\"\n    },\n    \"inLanguage\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"The language of the content.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  },\n  \"$defs\": {\n    \"Question\": {\n      \"type\": \"object\",\n      \"description\": \"A specific question.\",\n      \"required\": [\"@type\", \"name\", \"acceptedAnswer\"],\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"Question\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The full text of the question.\" },\n        \"acceptedAnswer\": {\n          \"$ref\": \"#/$defs/Answer\",\n          \"description\": \"The answer that has been accepted as best.\"\n        },\n        \"suggestedAnswer\": {\n          \"oneOf\": [\n            { \"$ref\": \"#/$defs/Answer\"\
  \ },\n            { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/Answer\" } }\n          ],\n          \"description\": \"An answer that is not accepted as best.\"\n        },\n        \"answerCount\": { \"type\": \"integer\", \"description\": \"The number of answers.\" },\n        \"upvoteCount\": { \"type\": \"integer\", \"description\": \"The number of upvotes.\" },\n        \"dateCreated\": { \"type\": \"string\", \"format\": \"date\", \"description\": \"The date the question was created.\" },\n        \"author\": {\n          \"oneOf\": [\n            { \"$ref\": \"schema-org-person-schema.json\" },\n            { \"$ref\": \"schema-org-organization-schema.json\" }\n          ],\n          \"description\": \"The author of the question.\"\n        }\n      }\n    },\n    \"Answer\": {\n      \"type\": \"object\",\n      \"description\": \"An answer offered to a question.\",\n      \"required\": [\"@type\", \"text\"],\n      \"properties\": {\n        \"@type\": { \"type\"\
  : \"string\", \"const\": \"Answer\" },\n        \"text\": { \"type\": \"string\", \"description\": \"The textual content of the answer.\" },\n        \"dateCreated\": { \"type\": \"string\", \"format\": \"date\", \"description\": \"The date the answer was created.\" },\n        \"upvoteCount\": { \"type\": \"integer\", \"description\": \"The number of upvotes.\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"URL of the answer.\" },\n        \"author\": {\n          \"oneOf\": [\n            { \"$ref\": \"schema-org-person-schema.json\" },\n            { \"$ref\": \"schema-org-organization-schema.json\" }\n          ],\n          \"description\": \"The author of the answer.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-faq-page-schema.json
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
title: Schema.org FAQPage
---
