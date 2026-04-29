---
description: Schema for an Adobe Lightroom album. Albums organize assets into user-defined collections within a catalog. Albums can be regular collections, collection sets (folders containing other albums), or projects.
layout: schema
name: Lightroom Album
properties_list:
- description: Unique identifier for the album (UUID format)
  name: id
  type: string
- description: Resource type identifier
  name: type
  type: string
- description: Album subtype determining its organizational role
  name: subtype
  type: string
- description: Server-side timestamp when the album was created
  name: created
  type: string
- description: Server-side timestamp when the album was last updated
  name: updated
  type: string
- description: Album metadata payload
  name: payload
  type: object
- description: ''
  name: links
  type: object
provider_name: Adobe Lightroom
provider_slug: lightroom
schema_file: json-schema/lightroom-album-schema.json
slug: lightroom-album
source_filename: lightroom-album-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://lr.adobe.io/schemas/lightroom/album.json\",\n  \"title\": \"Lightroom Album\",\n  \"description\": \"Schema for an Adobe Lightroom album. Albums organize assets into user-defined collections within a catalog. Albums can be regular collections, collection sets (folders containing other albums), or projects.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"type\",\n    \"subtype\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the album (UUID format)\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Resource type identifier\",\n      \"const\": \"album\"\n    },\n    \"subtype\": {\n      \"type\": \"string\",\n      \"description\": \"Album subtype determining its organizational role\",\n      \"enum\": [\n        \"collection\",\n        \"collection_set\",\n      \
  \  \"project\"\n      ]\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Server-side timestamp when the album was created\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Server-side timestamp when the album was last updated\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Album metadata payload\",\n      \"required\": [\n        \"name\"\n      ],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the album\"\n        },\n        \"userCreated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"User-side timestamp when the album was created\"\n        },\n        \"userUpdated\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"User-side\
  \ timestamp when the album was last updated\"\n        },\n        \"cover\": {\n          \"$ref\": \"#/$defs/CoverAsset\"\n        },\n        \"parent\": {\n          \"$ref\": \"#/$defs/ParentAlbum\"\n        }\n      }\n    },\n    \"links\": {\n      \"$ref\": \"#/$defs/Links\"\n    }\n  },\n  \"$defs\": {\n    \"CoverAsset\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the asset used as the album cover image\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Asset ID of the cover image\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"ParentAlbum\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the parent album for nested album organization\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Parent album ID (must be a collection_set)\"\n        }\n      },\n      \"required\": [\n\
  \        \"id\"\n      ]\n    },\n    \"Links\": {\n      \"type\": \"object\",\n      \"description\": \"HATEOAS navigation links\",\n      \"properties\": {\n        \"self\": {\n          \"$ref\": \"#/$defs/Link\"\n        },\n        \"assets\": {\n          \"$ref\": \"#/$defs/Link\"\n        }\n      },\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Link\"\n      }\n    },\n    \"Link\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"href\": {\n          \"type\": \"string\",\n          \"description\": \"URL of the linked resource\"\n        }\n      },\n      \"required\": [\n        \"href\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/json-schema/lightroom-album-schema.json
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
title: Lightroom Album
---
