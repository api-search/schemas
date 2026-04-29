---
description: A published component from a Figma team or file library. Published components are reusable design elements that can be shared across files and teams. This schema represents components as returned by the component endpoints of the Figma REST API.
layout: schema
name: Figma Published Component
properties_list:
- description: The globally unique identifier for the component. This key is stable across file versions and can be used to reference the component via the GET /v1/components/{key} endpoint.
  name: key
  type: string
- description: The unique identifier of the Figma file that contains this component.
  name: file_key
  type: string
- description: The unique identifier of the component node within the Figma file. The node_id combined with file_key can be used to construct a direct URL to the component.
  name: node_id
  type: string
- description: A URL to a thumbnail image of the component. Thumbnail URLs are temporary and expire after a period of time.
  name: thumbnail_url
  type: string
- description: The name of the component as it appears in the assets panel and library.
  name: name
  type: string
- description: The description of the component as entered by the publisher. Useful for documenting usage guidelines and design intent.
  name: description
  type: string
- description: The UTC ISO 8601 time when the component was first published to the library.
  name: created_at
  type: string
- description: The UTC ISO 8601 time when the component was last updated in the library.
  name: updated_at
  type: string
- description: ''
  name: user
  type: object
- description: ''
  name: containing_frame
  type: object
- description: If this component belongs to a component set (variant group), this is the ID of that component set.
  name: component_set_id
  type:
  - string
  - 'null'
- description: An array of documentation links attached to this component, providing external references to code, design specs, or other resources.
  name: documentation_links
  type: array
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-component-schema.json
slug: figma-component
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://figma.com/schemas/figma/component.json\",\n  \"title\": \"Figma Published Component\",\n  \"description\": \"A published component from a Figma team or file library. Published components are reusable design elements that can be shared across files and teams. This schema represents components as returned by the component endpoints of the Figma REST API.\",\n  \"type\": \"object\",\n  \"required\": [\"key\", \"file_key\", \"node_id\", \"name\", \"description\", \"created_at\", \"updated_at\", \"user\"],\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The globally unique identifier for the component. This key is stable across file versions and can be used to reference the component via the GET /v1/components/{key} endpoint.\"\n    },\n    \"file_key\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Figma file\
  \ that contains this component.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the component node within the Figma file. The node_id combined with file_key can be used to construct a direct URL to the component.\"\n    },\n    \"thumbnail_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL to a thumbnail image of the component. Thumbnail URLs are temporary and expire after a period of time.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the component as it appears in the assets panel and library.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the component as entered by the publisher. Useful for documenting usage guidelines and design intent.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The UTC ISO\
  \ 8601 time when the component was first published to the library.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The UTC ISO 8601 time when the component was last updated in the library.\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/User\"\n    },\n    \"containing_frame\": {\n      \"$ref\": \"#/$defs/FrameInfo\"\n    },\n    \"component_set_id\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"If this component belongs to a component set (variant group), this is the ID of that component set.\"\n    },\n    \"documentation_links\": {\n      \"type\": \"array\",\n      \"description\": \"An array of documentation links attached to this component, providing external references to code, design specs, or other resources.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DocumentationLink\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"User\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A Figma user who published or last updated the component.\",\n      \"required\": [\"id\", \"handle\", \"img_url\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique stable ID of the user.\"\n        },\n        \"handle\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the user.\"\n        },\n        \"img_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's profile image.\"\n        }\n      }\n    },\n    \"FrameInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the frame that contains the component in the Figma file. Provides context about where the component lives in the document structure.\",\n      \"properties\": {\n        \"nodeId\": {\n          \"type\": \"string\",\n          \"description\": \"The node ID of the containing frame.\"\n        },\n        \"name\": {\n    \
  \      \"type\": \"string\",\n          \"description\": \"The name of the containing frame.\"\n        },\n        \"backgroundColor\": {\n          \"type\": \"string\",\n          \"description\": \"The background color of the containing frame.\"\n        },\n        \"pageId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the page containing the frame.\"\n        },\n        \"pageName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the page containing the frame.\"\n        }\n      }\n    },\n    \"DocumentationLink\": {\n      \"type\": \"object\",\n      \"description\": \"A link to external documentation associated with the component.\",\n      \"required\": [\"uri\"],\n      \"properties\": {\n        \"uri\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URI of the documentation link.\"\n        }\n      }\n    },\n    \"ComponentSet\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"A published component set that groups variants of a component. Component sets enable designers to organize related component variations (e.g., different sizes, states, or themes) under a single parent.\",\n      \"required\": [\"key\", \"file_key\", \"node_id\", \"name\", \"description\", \"created_at\", \"updated_at\", \"user\"],\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The globally unique identifier for the component set.\"\n        },\n        \"file_key\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the Figma file containing the component set.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the component set node within the Figma file.\"\n        },\n        \"thumbnail_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\"\
  : \"A URL to a thumbnail image of the component set.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the component set.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The description of the component set as entered by the publisher.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The UTC ISO 8601 time when the component set was first published.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The UTC ISO 8601 time when the component set was last updated.\"\n        },\n        \"user\": {\n          \"$ref\": \"#/$defs/User\"\n        },\n        \"containing_frame\": {\n          \"$ref\": \"#/$defs/FrameInfo\"\n        }\n      }\n    },\n    \"PublishedStyle\": {\n      \"type\": \"\
  object\",\n      \"description\": \"A published style from a team or file library. Styles define reusable visual properties like colors, text formatting, effects, and layout grids.\",\n      \"required\": [\"key\", \"file_key\", \"node_id\", \"name\", \"description\", \"style_type\", \"created_at\", \"updated_at\", \"user\"],\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The globally unique identifier for the style.\"\n        },\n        \"file_key\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the Figma file containing the style.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier of the style node.\"\n        },\n        \"thumbnail_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"A URL to a thumbnail image of the style.\"\n        },\n        \"name\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The name of the style.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The description of the style.\"\n        },\n        \"style_type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of style.\",\n          \"enum\": [\"FILL\", \"TEXT\", \"EFFECT\", \"GRID\"]\n        },\n        \"sort_position\": {\n          \"type\": \"string\",\n          \"description\": \"A user-defined sort position for the style.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The UTC ISO 8601 time when the style was first published.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The UTC ISO 8601 time when the style was last updated.\"\n        },\n        \"user\": {\n  \
  \        \"$ref\": \"#/$defs/User\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-component-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: Figma Published Component
---
