---
description: Schema for an Adobe Lightroom asset rendition. Renditions are server-generated preview images derived from the master file with current develop settings applied. Available in multiple sizes from small thumbnails to full-resolution exports.
layout: schema
name: Lightroom Rendition
properties_list:
- description: Resource type identifier
  name: type
  type: string
- description: Size classification of the rendition. thumbnail2x is a small thumbnail, numeric values indicate the longest edge in pixels, and fullsize is the maximum available resolution.
  name: rendition_type
  type: string
- description: Unique identifier of the source asset
  name: asset_id
  type: string
- description: Unique identifier of the catalog containing the source asset
  name: catalog_id
  type: string
- description: Width of the rendition in pixels
  name: width
  type: integer
- description: Height of the rendition in pixels
  name: height
  type: integer
- description: MIME type of the rendition image
  name: contentType
  type: string
- description: Size of the rendition file in bytes
  name: contentLength
  type: integer
- description: Timestamp when the rendition was generated
  name: created
  type: string
- description: Timestamp when the rendition was last regenerated
  name: updated
  type: string
- description: ''
  name: links
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-rendition-schema.json
slug: lightroom-rendition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://lr.adobe.io/schemas/lightroom/rendition.json\",\n  \"title\": \"Lightroom Rendition\",\n  \"description\": \"Schema for an Adobe Lightroom asset rendition. Renditions are server-generated preview images derived from the master file with current develop settings applied. Available in multiple sizes from small thumbnails to full-resolution exports.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"type\",\n    \"rendition_type\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier\",\n      \"const\": \"rendition\"\n    },\n    \"rendition_type\": {\n      \"type\": \"string\",\n      \"description\": \"Size classification of the rendition. thumbnail2x is a small thumbnail, numeric values indicate the longest edge in pixels, and fullsize is the maximum available resolution.\",\n      \"enum\": [\n        \"thumbnail2x\"\
  ,\n        \"640\",\n        \"1024\",\n        \"2048\",\n        \"fullsize\"\n      ]\n    },\n    \"asset_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the source asset\"\n    },\n    \"catalog_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the catalog containing the source asset\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Width of the rendition in pixels\",\n      \"minimum\": 1\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Height of the rendition in pixels\",\n      \"minimum\": 1\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of the rendition image\",\n      \"const\": \"image/jpeg\"\n    },\n    \"contentLength\": {\n      \"type\": \"integer\",\n      \"description\": \"Size of the rendition file in bytes\",\n      \"minimum\": 0\n    },\n    \"created\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the rendition was generated\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the rendition was last regenerated\"\n    },\n    \"links\": {\n      \"$ref\": \"#/$defs/Links\"\n    }\n  },\n  \"$defs\": {\n    \"Links\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation links\",\n      \"properties\": {\n        \"self\": {\n          \"$ref\": \"#/$defs/Link\"\n        },\n        \"asset\": {\n          \"$ref\": \"#/$defs/Link\"\n        }\n      },\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    },\n    \"Link\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"description\": \"URL of the linked resource\"\n        }\n      },\n      \"required\": [\n        \"href\"\n      ]\n    }\n  }\n\
  }\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-rendition-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: Lightroom Rendition
---
