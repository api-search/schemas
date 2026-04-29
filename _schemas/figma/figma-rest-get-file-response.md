---
description: Response from the Get File endpoint.
layout: schema
name: GetFileResponse
properties_list:
- description: The name of the file as it appears in the editor.
  name: name
  type: string
- description: The role of the requesting user in relation to the file.
  name: role
  type: string
- description: The UTC ISO 8601 time at which the file was last modified.
  name: lastModified
  type: string
- description: The type of editor associated with this file.
  name: editorType
  type: string
- description: A URL to a thumbnail image of the file.
  name: thumbnailUrl
  type: string
- description: The version number of the file.
  name: version
  type: string
- description: A mapping from component IDs to component metadata.
  name: components
  type: object
- description: A mapping from component set IDs to component set metadata.
  name: componentSets
  type: object
- description: The schema version of the file format.
  name: schemaVersion
  type: integer
- description: A mapping from style IDs to style metadata.
  name: styles
  type: object
- description: The key of the main file, if this is a branch.
  name: mainFileKey
  type: string
- description: A list of branches for this file.
  name: branches
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-get-file-response-schema.json
slug: figma-rest-get-file-response
source_filename: figma-rest-get-file-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetFileResponse\",\n  \"type\": \"object\",\n  \"description\": \"Response from the Get File endpoint.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the file as it appears in the editor.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"description\": \"The role of the requesting user in relation to the file.\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time at which the file was last modified.\"\n    },\n    \"editorType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of editor associated with this file.\"\n    },\n    \"thumbnailUrl\": {\n      \"type\": \"string\",\n      \"description\": \"A URL to a thumbnail image of the file.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version number\
  \ of the file.\"\n    },\n    \"components\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping from component IDs to component metadata.\"\n    },\n    \"componentSets\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping from component set IDs to component set metadata.\"\n    },\n    \"schemaVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"The schema version of the file format.\"\n    },\n    \"styles\": {\n      \"type\": \"object\",\n      \"description\": \"A mapping from style IDs to style metadata.\"\n    },\n    \"mainFileKey\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the main file, if this is a branch.\"\n    },\n    \"branches\": {\n      \"type\": \"array\",\n      \"description\": \"A list of branches for this file.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-get-file-response-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: GetFileResponse
---
