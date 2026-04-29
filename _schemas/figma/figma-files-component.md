---
description: A description of a main component.
layout: schema
name: Component
properties_list:
- description: The key of the component.
  name: key
  type: string
- description: Name of the component.
  name: name
  type: string
- description: The description of the component as entered in the editor.
  name: description
  type: string
- description: The ID of the component set if the component belongs to one.
  name: componentSetId
  type: string
- description: An array of documentation links attached to this component.
  name: documentationLinks
  type: array
- description: Whether this component is a remote component.
  name: remote
  type: boolean
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-files-component-schema.json
slug: figma-files-component
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Component\",\n  \"type\": \"object\",\n  \"description\": \"A description of a main component.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the component.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the component.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the component as entered in the editor.\"\n    },\n    \"componentSetId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the component set if the component belongs to one.\"\n    },\n    \"documentationLinks\": {\n      \"type\": \"array\",\n      \"description\": \"An array of documentation links attached to this component.\"\n    },\n    \"remote\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this component is a remote component.\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-files-component-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Component
---
