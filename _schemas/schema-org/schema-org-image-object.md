---
description: An image file.
layout: schema
name: Schema.org ImageObject
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: URL of the image.
  name: url
  type: string
- description: Actual bytes of the media object.
  name: contentUrl
  type: string
- description: The name of the image.
  name: name
  type: string
- description: A description of the image.
  name: description
  type: string
- description: The caption for this image.
  name: caption
  type: string
- description: The width of the image in pixels.
  name: width
  type: object
- description: The height of the image in pixels.
  name: height
  type: object
- description: Media type expressed using a MIME format (e.g., image/jpeg, image/png).
  name: encodingFormat
  type: string
- description: File size in bytes.
  name: contentSize
  type: string
- description: Thumbnail image.
  name: thumbnail
  type: object
- description: Indicates whether this image is representative of the content of the page.
  name: representativeOfPage
  type: boolean
- description: EXIF data for the image.
  name: exifData
  type: array
- description: The author of this image.
  name: author
  type: object
- description: The party holding the legal copyright.
  name: copyrightHolder
  type: object
- description: The year during which the claimed copyright was first asserted.
  name: copyrightYear
  type: integer
- description: A license document that applies to this image.
  name: license
  type: string
- description: URL to acquire a license for using the image.
  name: acquireLicensePage
  type: string
- description: Text that can be used to credit person(s) and/or organization(s) associated with the image.
  name: creditText
  type: string
- description: Date of first publication.
  name: datePublished
  type: string
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-image-object-schema.json
slug: schema-org-image-object
source_filename: schema-org-image-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/image-object.json\",\n  \"title\": \"Schema.org ImageObject\",\n  \"description\": \"An image file.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"const\": \"ImageObject\",\n      \"description\": \"The Schema.org type.\"\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the image.\"\n    },\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Actual bytes of the media object.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the image.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"\
  A description of the image.\"\n    },\n    \"caption\": {\n      \"type\": \"string\",\n      \"description\": \"The caption for this image.\"\n    },\n    \"width\": {\n      \"oneOf\": [\n        { \"type\": \"integer\" },\n        { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"QuantitativeValue\" }, \"value\": { \"type\": \"integer\" }, \"unitCode\": { \"type\": \"string\" } } }\n      ],\n      \"description\": \"The width of the image in pixels.\"\n    },\n    \"height\": {\n      \"oneOf\": [\n        { \"type\": \"integer\" },\n        { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"QuantitativeValue\" }, \"value\": { \"type\": \"integer\" }, \"unitCode\": { \"type\": \"string\" } } }\n      ],\n      \"description\": \"The height of the image in pixels.\"\n    },\n    \"encodingFormat\": {\n      \"type\": \"string\",\n      \"description\": \"Media type expressed using a MIME format (e.g., image/jpeg, image/png).\"\n    },\n    \"contentSize\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"File size in bytes.\"\n    },\n    \"thumbnail\": {\n      \"$ref\": \"#\",\n      \"description\": \"Thumbnail image.\"\n    },\n    \"representativeOfPage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this image is representative of the content of the page.\"\n    },\n    \"exifData\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"schema-org-property-value-schema.json\" },\n      \"description\": \"EXIF data for the image.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The author of this image.\"\n    },\n    \"copyrightHolder\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The party holding\
  \ the legal copyright.\"\n    },\n    \"copyrightYear\": {\n      \"type\": \"integer\",\n      \"description\": \"The year during which the claimed copyright was first asserted.\"\n    },\n    \"license\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A license document that applies to this image.\"\n    },\n    \"acquireLicensePage\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to acquire a license for using the image.\"\n    },\n    \"creditText\": {\n      \"type\": \"string\",\n      \"description\": \"Text that can be used to credit person(s) and/or organization(s) associated with the image.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\"\
  , \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-image-object-schema.json
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
title: Schema.org ImageObject
---
