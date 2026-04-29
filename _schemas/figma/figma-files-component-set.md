---
description: A description of a component set.
layout: schema
name: ComponentSet
properties_list:
- description: The key of the component set.
  name: key
  type: string
- description: Name of the component set.
  name: name
  type: string
- description: The description of the component set as entered in the editor.
  name: description
  type: string
- description: An array of documentation links attached to this component set.
  name: documentationLinks
  type: array
- description: Whether this component set is a remote component set.
  name: remote
  type: boolean
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-files-component-set-schema.json
slug: figma-files-component-set
source_filename: figma-files-component-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComponentSet\",\n  \"type\": \"object\",\n  \"description\": \"A description of a component set.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the component set.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the component set.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the component set as entered in the editor.\"\n    },\n    \"documentationLinks\": {\n      \"type\": \"array\",\n      \"description\": \"An array of documentation links attached to this component set.\"\n    },\n    \"remote\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this component set is a remote component set.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-files-component-set-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: ComponentSet
---
