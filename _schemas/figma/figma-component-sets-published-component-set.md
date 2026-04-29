---
description: A node containing a set of variants of a component.
layout: schema
name: PublishedComponentSet
properties_list:
- description: The unique identifier for the component set.
  name: key
  type: string
- description: The unique identifier of the Figma file that contains the component set.
  name: fileKey
  type: string
- description: The unique identifier of the component set node within the Figma file.
  name: nodeId
  type: string
- description: A URL to a thumbnail image of the component set.
  name: thumbnailUrl
  type: string
- description: The name of the component set.
  name: name
  type: string
- description: The description of the component set as entered by the publisher.
  name: description
  type: string
- description: The UTC ISO 8601 time when the component set was created.
  name: createdAt
  type: string
- description: The UTC ISO 8601 time when the component set was last updated.
  name: updatedAt
  type: string
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-component-sets-published-component-set-schema.json
slug: figma-component-sets-published-component-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublishedComponentSet\",\n  \"type\": \"object\",\n  \"description\": \"A node containing a set of variants of a component.\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the component set.\"\n    },\n    \"fileKey\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Figma file that contains the component set.\"\n    },\n    \"nodeId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the component set node within the Figma file.\"\n    },\n    \"thumbnailUrl\": {\n      \"type\": \"string\",\n      \"description\": \"A URL to a thumbnail image of the component set.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the component set.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The description of the component set as entered by the publisher.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time when the component set was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The UTC ISO 8601 time when the component set was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-component-sets-published-component-set-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: PublishedComponentSet
---
