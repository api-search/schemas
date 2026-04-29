---
description: A published component from a team or file library.
layout: schema
name: PublishedComponent
properties_list:
- description: The globally unique identifier for the component.
  name: key
  type: string
- description: The key of the Figma file containing the component.
  name: file_key
  type: string
- description: The node ID of the component within the file.
  name: node_id
  type: string
- description: A URL to a thumbnail image of the component.
  name: thumbnail_url
  type: string
- description: The name of the component.
  name: name
  type: string
- description: The description of the component as entered by the publisher.
  name: description
  type: string
- description: The UTC ISO 8601 time when the component was first published.
  name: created_at
  type: string
- description: The UTC ISO 8601 time when the component was last updated.
  name: updated_at
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-published-component-schema.json
slug: figma-rest-published-component
source_filename: figma-rest-published-component-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublishedComponent\",\n  \"type\": \"object\",\n  \"description\": \"A published component from a team or file library.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The globally unique identifier for the component.\"\n    },\n    \"file_key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the Figma file containing the component.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The node ID of the component within the file.\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"description\": \"A URL to a thumbnail image of the component.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the component.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the component as\
  \ entered by the publisher.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time when the component was first published.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time when the component was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-published-component-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: PublishedComponent
---
