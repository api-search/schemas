---
description: Instructions that explain how to achieve a result by performing a sequence of steps.
layout: schema
name: Schema.org HowTo
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the how-to guide.
  name: name
  type: string
- description: A description of the how-to guide.
  name: description
  type: string
- description: URL of the how-to guide.
  name: url
  type: string
- description: An image of the completed how-to.
  name: image
  type: object
- description: The total time required to perform all steps in ISO 8601 duration format.
  name: totalTime
  type: string
- description: The length of time it takes to prepare the items in ISO 8601 duration format.
  name: prepTime
  type: string
- description: The length of time it takes to perform instructions in ISO 8601 duration format.
  name: performTime
  type: string
- description: The estimated cost of the supply or supplies consumed when performing instructions.
  name: estimatedCost
  type: object
- description: A sub-property of instrument. A supply consumed when performing instructions or a direction.
  name: supply
  type: object
- description: A sub-property of instrument. An object used (but not consumed) when performing instructions.
  name: tool
  type: object
- description: The steps in the how-to.
  name: step
  type: array
- description: The quantity that results by performing instructions.
  name: yield
  type: string
- description: The author of this how-to guide.
  name: author
  type: object
- description: Date of first publication.
  name: datePublished
  type: string
- description: A video of the how-to.
  name: video
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-how-to-schema.json
slug: schema-org-how-to
source_filename: schema-org-how-to-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/how-to.json\",\n  \"title\": \"Schema.org HowTo\",\n  \"description\": \"Instructions that explain how to achieve a result by performing a sequence of steps.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\", \"step\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"HowTo\", \"Recipe\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the how-to guide.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the how-to guide.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the how-to guide.\"\n    },\n   \
  \ \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the completed how-to.\"\n    },\n    \"totalTime\": {\n      \"type\": \"string\",\n      \"description\": \"The total time required to perform all steps in ISO 8601 duration format.\"\n    },\n    \"prepTime\": {\n      \"type\": \"string\",\n      \"description\": \"The length of time it takes to prepare the items in ISO 8601 duration format.\"\n    },\n    \"performTime\": {\n      \"type\": \"string\",\n      \"description\": \"The length of time it takes to perform instructions in ISO 8601 duration format.\"\n    },\n    \"estimatedCost\": {\n      \"type\": \"object\",\n      \"description\": \"The estimated cost of the supply or supplies consumed when performing instructions.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"MonetaryAmount\" },\n\
  \        \"currency\": { \"type\": \"string\" },\n        \"value\": { \"type\": \"number\" }\n      }\n    },\n    \"supply\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/HowToSupply\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/HowToSupply\" } }\n      ],\n      \"description\": \"A sub-property of instrument. A supply consumed when performing instructions or a direction.\"\n    },\n    \"tool\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/HowToTool\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/HowToTool\" } }\n      ],\n      \"description\": \"A sub-property of instrument. An object used (but not consumed) when performing instructions.\"\n    },\n    \"step\": {\n      \"type\": \"array\",\n      \"description\": \"The steps in the how-to.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/HowToStep\"\n      }\n    },\n    \"yield\": {\n      \"type\": \"string\",\n      \"description\": \"The quantity that results\
  \ by performing instructions.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The author of this how-to guide.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"video\": {\n      \"$ref\": \"schema-org-video-object-schema.json\",\n      \"description\": \"A video of the how-to.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  },\n  \"$defs\": {\n    \"HowToStep\": {\n      \"type\": \"object\",\n      \"description\": \"A step in the instructions for\
  \ how to achieve a result.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"HowToStep\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the step.\" },\n        \"text\": { \"type\": \"string\", \"description\": \"The text directions for the step.\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"A URL linking to the step.\" },\n        \"image\": { \"oneOf\": [{ \"type\": \"string\", \"format\": \"uri\" }, { \"$ref\": \"schema-org-image-object-schema.json\" }], \"description\": \"An image for the step.\" },\n        \"position\": { \"type\": \"integer\", \"description\": \"The position of the step.\" },\n        \"itemListElement\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"@type\": { \"const\": \"HowToDirection\" },\n              \"text\": { \"type\": \"string\" }\n            }\n     \
  \     },\n          \"description\": \"Detailed elements of this step.\"\n        }\n      }\n    },\n    \"HowToSupply\": {\n      \"type\": \"object\",\n      \"description\": \"A supply consumed when performing instructions.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"HowToSupply\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the supply.\" },\n        \"requiredQuantity\": { \"type\": \"number\", \"description\": \"The required quantity.\" },\n        \"image\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"An image of the supply.\" },\n        \"estimatedCost\": { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"MonetaryAmount\" }, \"currency\": { \"type\": \"string\" }, \"value\": { \"type\": \"number\" } } }\n      }\n    },\n    \"HowToTool\": {\n      \"type\": \"object\",\n      \"description\": \"A tool used (but not consumed) when performing instructions.\",\n      \"\
  properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"HowToTool\" },\n        \"name\": { \"type\": \"string\", \"description\": \"The name of the tool.\" },\n        \"image\": { \"type\": \"string\", \"format\": \"uri\", \"description\": \"An image of the tool.\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-how-to-schema.json
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
title: Schema.org HowTo
---
