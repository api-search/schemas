---
description: A Block object represents a piece of content within a Notion page. Blocks are the fundamental building units of all page content. They can be paragraphs, headings, lists, images, code, tables, and many other types. Blocks can contain child blocks, forming a tree structure.
layout: schema
name: Notion Block
properties_list:
- description: Always 'block' for block objects.
  name: object
  type: string
- description: Unique identifier for the block (UUIDv4).
  name: id
  type: string
- description: The parent of the block (page, block, or database).
  name: parent
  type: object
- description: The type of block. Determines which type-specific content field is populated on this object.
  name: type
  type: string
- description: Date and time when the block was created, in ISO 8601 format.
  name: created_time
  type: string
- description: Date and time when the block was last edited, in ISO 8601 format.
  name: last_edited_time
  type: string
- description: The user who created the block.
  name: created_by
  type: object
- description: The user who last edited the block.
  name: last_edited_by
  type: object
- description: Whether the block has been archived (deleted).
  name: archived
  type: boolean
- description: Whether the block is in the trash.
  name: in_trash
  type: boolean
- description: Whether the block has child blocks nested within it.
  name: has_children
  type: boolean
- description: Paragraph content. Present when type is 'paragraph'.
  name: paragraph
  type: object
- description: Heading 1 content. Present when type is 'heading_1'.
  name: heading_1
  type: object
- description: Heading 2 content. Present when type is 'heading_2'.
  name: heading_2
  type: object
- description: Heading 3 content. Present when type is 'heading_3'.
  name: heading_3
  type: object
- description: Bulleted list item content. Present when type is 'bulleted_list_item'.
  name: bulleted_list_item
  type: object
- description: Numbered list item content. Present when type is 'numbered_list_item'.
  name: numbered_list_item
  type: object
- description: To-do item content. Present when type is 'to_do'.
  name: to_do
  type: object
- description: Toggle content. Present when type is 'toggle'.
  name: toggle
  type: object
- description: Child page reference. Present when type is 'child_page'.
  name: child_page
  type: object
- description: Child database reference. Present when type is 'child_database'.
  name: child_database
  type: object
- description: Embed content. Present when type is 'embed'.
  name: embed
  type: object
- description: Image content. Present when type is 'image'.
  name: image
  type: object
- description: Video content. Present when type is 'video'.
  name: video
  type: object
- description: File content. Present when type is 'file'.
  name: file
  type: object
- description: PDF content. Present when type is 'pdf'.
  name: pdf
  type: object
- description: Audio content. Present when type is 'audio'.
  name: audio
  type: object
- description: Bookmark content. Present when type is 'bookmark'.
  name: bookmark
  type: object
- description: Callout content. Present when type is 'callout'.
  name: callout
  type: object
- description: Quote content. Present when type is 'quote'.
  name: quote
  type: object
- description: Equation (KaTeX) content. Present when type is 'equation'.
  name: equation
  type: object
- description: Divider block (empty object). Present when type is 'divider'.
  name: divider
  type: object
- description: Table of contents block. Present when type is 'table_of_contents'.
  name: table_of_contents
  type: object
- description: Code block content. Present when type is 'code'.
  name: code
  type: object
- description: Table block configuration. Present when type is 'table'.
  name: table
  type: object
- description: Table row content. Present when type is 'table_row'.
  name: table_row
  type: object
- description: Synced block content. Present when type is 'synced_block'.
  name: synced_block
  type: object
- description: Link preview content. Present when type is 'link_preview'.
  name: link_preview
  type: object
- description: Link to page content. Present when type is 'link_to_page'.
  name: link_to_page
  type: object
- description: Breadcrumb block (empty object). Present when type is 'breadcrumb'.
  name: breadcrumb
  type: object
- description: Column list block. Present when type is 'column_list'. Children are column blocks.
  name: column_list
  type: object
- description: Column block. Present when type is 'column'. Children are the blocks in the column.
  name: column
  type: object
- description: Template block content. Present when type is 'template'.
  name: template
  type: object
provider_name: Notion
provider_slug: notion
schema_file: json-schema/notion-block-schema.json
slug: notion-block
source_filename: notion-block-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/json-schema/notion-block-schema.json\",\n  \"title\": \"Notion Block\",\n  \"description\": \"A Block object represents a piece of content within a Notion page. Blocks are the fundamental building units of all page content. They can be paragraphs, headings, lists, images, code, tables, and many other types. Blocks can contain child blocks, forming a tree structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"block\",\n      \"description\": \"Always 'block' for block objects.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the block (UUIDv4).\"\n    },\n    \"parent\": {\n      \"$ref\": \"#/$defs/Parent\",\n      \"description\": \"The parent of the block (page, block,\
  \ or database).\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of block. Determines which type-specific content field is populated on this object.\",\n      \"enum\": [\n        \"paragraph\",\n        \"heading_1\",\n        \"heading_2\",\n        \"heading_3\",\n        \"bulleted_list_item\",\n        \"numbered_list_item\",\n        \"to_do\",\n        \"toggle\",\n        \"child_page\",\n        \"child_database\",\n        \"embed\",\n        \"image\",\n        \"video\",\n        \"file\",\n        \"pdf\",\n        \"bookmark\",\n        \"callout\",\n        \"quote\",\n        \"equation\",\n        \"divider\",\n        \"table_of_contents\",\n        \"column_list\",\n        \"column\",\n        \"link_preview\",\n        \"synced_block\",\n        \"template\",\n        \"link_to_page\",\n        \"table\",\n        \"table_row\",\n        \"code\",\n        \"audio\",\n        \"breadcrumb\"\n      ]\n    },\n    \"created_time\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the block was created, in ISO 8601 format.\"\n    },\n    \"last_edited_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the block was last edited, in ISO 8601 format.\"\n    },\n    \"created_by\": {\n      \"$ref\": \"#/$defs/PartialUser\",\n      \"description\": \"The user who created the block.\"\n    },\n    \"last_edited_by\": {\n      \"$ref\": \"#/$defs/PartialUser\",\n      \"description\": \"The user who last edited the block.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the block has been archived (deleted).\"\n    },\n    \"in_trash\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the block is in the trash.\"\n    },\n    \"has_children\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the block has child blocks\
  \ nested within it.\"\n    },\n    \"paragraph\": {\n      \"$ref\": \"#/$defs/TextBlock\",\n      \"description\": \"Paragraph content. Present when type is 'paragraph'.\"\n    },\n    \"heading_1\": {\n      \"$ref\": \"#/$defs/HeadingBlock\",\n      \"description\": \"Heading 1 content. Present when type is 'heading_1'.\"\n    },\n    \"heading_2\": {\n      \"$ref\": \"#/$defs/HeadingBlock\",\n      \"description\": \"Heading 2 content. Present when type is 'heading_2'.\"\n    },\n    \"heading_3\": {\n      \"$ref\": \"#/$defs/HeadingBlock\",\n      \"description\": \"Heading 3 content. Present when type is 'heading_3'.\"\n    },\n    \"bulleted_list_item\": {\n      \"$ref\": \"#/$defs/TextBlock\",\n      \"description\": \"Bulleted list item content. Present when type is 'bulleted_list_item'.\"\n    },\n    \"numbered_list_item\": {\n      \"$ref\": \"#/$defs/TextBlock\",\n      \"description\": \"Numbered list item content. Present when type is 'numbered_list_item'.\"\n    },\n\
  \    \"to_do\": {\n      \"type\": \"object\",\n      \"description\": \"To-do item content. Present when type is 'to_do'.\",\n      \"properties\": {\n        \"rich_text\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/RichText\" }\n        },\n        \"checked\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the to-do is checked.\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"The color of the block.\"\n        },\n        \"children\": {\n          \"type\": \"array\",\n          \"description\": \"Nested child blocks.\",\n          \"items\": { \"$ref\": \"#\" }\n        }\n      }\n    },\n    \"toggle\": {\n      \"$ref\": \"#/$defs/TextBlock\",\n      \"description\": \"Toggle content. Present when type is 'toggle'.\"\n    },\n    \"child_page\": {\n      \"type\": \"object\",\n      \"description\": \"Child page reference. Present when type is 'child_page'.\",\n    \
  \  \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The title of the child page.\"\n        }\n      },\n      \"required\": [\"title\"]\n    },\n    \"child_database\": {\n      \"type\": \"object\",\n      \"description\": \"Child database reference. Present when type is 'child_database'.\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The title of the child database.\"\n        }\n      },\n      \"required\": [\"title\"]\n    },\n    \"embed\": {\n      \"type\": \"object\",\n      \"description\": \"Embed content. Present when type is 'embed'.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the embedded content.\"\n        },\n        \"caption\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/RichText\" }\n        }\n      }\n \
  \   },\n    \"image\": {\n      \"$ref\": \"#/$defs/FileBlock\",\n      \"description\": \"Image content. Present when type is 'image'.\"\n    },\n    \"video\": {\n      \"$ref\": \"#/$defs/FileBlock\",\n      \"description\": \"Video content. Present when type is 'video'.\"\n    },\n    \"file\": {\n      \"$ref\": \"#/$defs/FileBlock\",\n      \"description\": \"File content. Present when type is 'file'.\"\n    },\n    \"pdf\": {\n      \"$ref\": \"#/$defs/FileBlock\",\n      \"description\": \"PDF content. Present when type is 'pdf'.\"\n    },\n    \"audio\": {\n      \"$ref\": \"#/$defs/FileBlock\",\n      \"description\": \"Audio content. Present when type is 'audio'.\"\n    },\n    \"bookmark\": {\n      \"type\": \"object\",\n      \"description\": \"Bookmark content. Present when type is 'bookmark'.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the bookmarked page.\"\n \
  \       },\n        \"caption\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/RichText\" }\n        }\n      },\n      \"required\": [\"url\"]\n    },\n    \"callout\": {\n      \"type\": \"object\",\n      \"description\": \"Callout content. Present when type is 'callout'.\",\n      \"properties\": {\n        \"rich_text\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/RichText\" }\n        },\n        \"icon\": {\n          \"oneOf\": [\n            { \"$ref\": \"#/$defs/Emoji\" },\n            { \"$ref\": \"#/$defs/File\" }\n          ]\n        },\n        \"color\": {\n          \"type\": \"string\"\n        },\n        \"children\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#\" }\n        }\n      }\n    },\n    \"quote\": {\n      \"$ref\": \"#/$defs/TextBlock\",\n      \"description\": \"Quote content. Present when type is 'quote'.\"\n    },\n    \"equation\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Equation (KaTeX) content. Present when type is 'equation'.\",\n      \"properties\": {\n        \"expression\": {\n          \"type\": \"string\",\n          \"description\": \"The LaTeX equation expression.\"\n        }\n      },\n      \"required\": [\"expression\"]\n    },\n    \"divider\": {\n      \"type\": \"object\",\n      \"description\": \"Divider block (empty object). Present when type is 'divider'.\"\n    },\n    \"table_of_contents\": {\n      \"type\": \"object\",\n      \"description\": \"Table of contents block. Present when type is 'table_of_contents'.\",\n      \"properties\": {\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"The color of the block.\"\n        }\n      }\n    },\n    \"code\": {\n      \"type\": \"object\",\n      \"description\": \"Code block content. Present when type is 'code'.\",\n      \"properties\": {\n        \"rich_text\": {\n          \"type\": \"array\",\n          \"items\":\
  \ { \"$ref\": \"#/$defs/RichText\" }\n        },\n        \"caption\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/RichText\" }\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"The programming language of the code block.\"\n        }\n      }\n    },\n    \"table\": {\n      \"type\": \"object\",\n      \"description\": \"Table block configuration. Present when type is 'table'.\",\n      \"properties\": {\n        \"table_width\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of columns in the table.\"\n        },\n        \"has_column_header\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the first row is a header.\"\n        },\n        \"has_row_header\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the first column is a header.\"\n        }\n      }\n    },\n    \"table_row\": {\n      \"type\": \"object\",\n     \
  \ \"description\": \"Table row content. Present when type is 'table_row'.\",\n      \"properties\": {\n        \"cells\": {\n          \"type\": \"array\",\n          \"description\": \"Array of cell contents. Each cell is an array of rich text.\",\n          \"items\": {\n            \"type\": \"array\",\n            \"items\": { \"$ref\": \"#/$defs/RichText\" }\n          }\n        }\n      }\n    },\n    \"synced_block\": {\n      \"type\": \"object\",\n      \"description\": \"Synced block content. Present when type is 'synced_block'.\",\n      \"properties\": {\n        \"synced_from\": {\n          \"type\": [\"object\", \"null\"],\n          \"description\": \"Reference to the original synced block, or null if this is the original.\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"const\": \"block_id\"\n            },\n            \"block_id\": {\n              \"type\": \"string\",\n              \"format\": \"uuid\"\
  \n            }\n          }\n        },\n        \"children\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#\" }\n        }\n      }\n    },\n    \"link_preview\": {\n      \"type\": \"object\",\n      \"description\": \"Link preview content. Present when type is 'link_preview'.\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      }\n    },\n    \"link_to_page\": {\n      \"type\": \"object\",\n      \"description\": \"Link to page content. Present when type is 'link_to_page'.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"page_id\", \"database_id\"]\n        },\n        \"page_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"database_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        }\n      }\n    },\n    \"breadcrumb\": {\n      \"type\": \"object\"\
  ,\n      \"description\": \"Breadcrumb block (empty object). Present when type is 'breadcrumb'.\"\n    },\n    \"column_list\": {\n      \"type\": \"object\",\n      \"description\": \"Column list block. Present when type is 'column_list'. Children are column blocks.\",\n      \"properties\": {\n        \"children\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#\" }\n        }\n      }\n    },\n    \"column\": {\n      \"type\": \"object\",\n      \"description\": \"Column block. Present when type is 'column'. Children are the blocks in the column.\",\n      \"properties\": {\n        \"children\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#\" }\n        }\n      }\n    },\n    \"template\": {\n      \"type\": \"object\",\n      \"description\": \"Template block content. Present when type is 'template'.\",\n      \"properties\": {\n        \"rich_text\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/RichText\"\
  \ }\n        },\n        \"children\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#\" }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"id\",\n    \"type\",\n    \"created_time\",\n    \"last_edited_time\",\n    \"has_children\"\n  ],\n  \"additionalProperties\": true,\n  \"$defs\": {\n    \"PartialUser\": {\n      \"type\": \"object\",\n      \"description\": \"A partial user reference containing only the object type and ID.\",\n      \"properties\": {\n        \"object\": {\n          \"type\": \"string\",\n          \"const\": \"user\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        }\n      },\n      \"required\": [\"object\", \"id\"]\n    },\n    \"Parent\": {\n      \"type\": \"object\",\n      \"description\": \"The parent of a block.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"database_id\", \"page_id\", \"\
  block_id\", \"workspace\"]\n        },\n        \"database_id\": { \"type\": \"string\", \"format\": \"uuid\" },\n        \"page_id\": { \"type\": \"string\", \"format\": \"uuid\" },\n        \"block_id\": { \"type\": \"string\", \"format\": \"uuid\" },\n        \"workspace\": { \"type\": \"boolean\" }\n      },\n      \"required\": [\"type\"]\n    },\n    \"RichText\": {\n      \"type\": \"object\",\n      \"description\": \"A rich text element with content, styling annotations, and optional links.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"text\", \"mention\", \"equation\"]\n        },\n        \"text\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"content\": { \"type\": \"string\" },\n            \"link\": {\n              \"type\": [\"object\", \"null\"],\n              \"properties\": {\n                \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n              }\n         \
  \   }\n          }\n        },\n        \"mention\": {\n          \"type\": \"object\",\n          \"description\": \"Mention content for referencing users, pages, databases, dates, or links.\",\n          \"additionalProperties\": true\n        },\n        \"equation\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"expression\": { \"type\": \"string\" }\n          }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"bold\": { \"type\": \"boolean\" },\n            \"italic\": { \"type\": \"boolean\" },\n            \"strikethrough\": { \"type\": \"boolean\" },\n            \"underline\": { \"type\": \"boolean\" },\n            \"code\": { \"type\": \"boolean\" },\n            \"color\": { \"type\": \"string\" }\n          }\n        },\n        \"plain_text\": { \"type\": \"string\" },\n        \"href\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\"\n     \
  \   }\n      },\n      \"required\": [\"type\", \"plain_text\"]\n    },\n    \"Emoji\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": { \"type\": \"string\", \"const\": \"emoji\" },\n        \"emoji\": { \"type\": \"string\" }\n      },\n      \"required\": [\"type\", \"emoji\"]\n    },\n    \"File\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"file\", \"external\"]\n        },\n        \"file\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n            \"expiry_time\": { \"type\": \"string\", \"format\": \"date-time\" }\n          }\n        },\n        \"external\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n          }\n        }\n      },\n      \"required\": [\"type\"]\n    },\n    \"TextBlock\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"A text-based block containing rich text, color, and optional children.\",\n      \"properties\": {\n        \"rich_text\": {\n          \"type\": \"array\",\n          \"description\": \"The rich text content of the block.\",\n          \"items\": { \"$ref\": \"#/$defs/RichText\" }\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"The color of the block text or background.\"\n        },\n        \"children\": {\n          \"type\": \"array\",\n          \"description\": \"Nested child blocks.\",\n          \"items\": { \"$ref\": \"#\" }\n        }\n      }\n    },\n    \"HeadingBlock\": {\n      \"type\": \"object\",\n      \"description\": \"A heading block containing rich text and toggle information.\",\n      \"properties\": {\n        \"rich_text\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/RichText\" }\n        },\n        \"color\": {\n   \
  \       \"type\": \"string\"\n        },\n        \"is_toggleable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the heading is a toggleable heading.\"\n        }\n      }\n    },\n    \"FileBlock\": {\n      \"type\": \"object\",\n      \"description\": \"A file-based block (image, video, file, pdf, audio).\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"file\", \"external\"],\n          \"description\": \"Whether the file is Notion-hosted or external.\"\n        },\n        \"file\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n            \"expiry_time\": { \"type\": \"string\", \"format\": \"date-time\" }\n          }\n        },\n        \"external\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n          }\n        },\n\
  \        \"caption\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/RichText\" }\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\"type\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/json-schema/notion-block-schema.json
tags:
- Collaboration
- Database
- Ideas
- Notes
- Productivity
- Projects
- T1
- Tasks
- Wiki
- Workspace
title: Notion Block
---
