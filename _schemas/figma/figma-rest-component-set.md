---
description: A component set groups variants of a component together. Useful for organizing different states or configurations of a design element.
layout: schema
name: ComponentSet
properties_list:
- description: The globally unique key of the component set.
  name: key
  type: string
- description: Name of the component set.
  name: name
  type: string
- description: The description of the component set as entered in the editor.
  name: description
  type: string
- description: Documentation links attached to this component set.
  name: documentationLinks
  type: array
- description: Whether this is a remote component set.
  name: remote
  type: boolean
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-rest-component-set-schema.json
slug: figma-rest-component-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComponentSet\",\n  \"type\": \"object\",\n  \"description\": \"A component set groups variants of a component together. Useful for organizing different states or configurations of a design element.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The globally unique key of the component set.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the component set.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the component set as entered in the editor.\"\n    },\n    \"documentationLinks\": {\n      \"type\": \"array\",\n      \"description\": \"Documentation links attached to this component set.\"\n    },\n    \"remote\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a remote component set.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-rest-component-set-schema.json
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
