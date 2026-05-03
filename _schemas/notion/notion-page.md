---
description: A Page object represents a page in a Notion workspace. Pages can exist as standalone pages in a workspace or as items within a database. Each page has properties (metadata fields) and content composed of blocks.
layout: schema
name: Notion Page
properties_list:
- description: Always 'page' for page objects.
  name: object
  type: string
- description: Unique identifier for the page (UUIDv4).
  name: id
  type: string
- description: Date and time when the page was created, in ISO 8601 format.
  name: created_time
  type: string
- description: Date and time when the page was last edited, in ISO 8601 format.
  name: last_edited_time
  type: string
- description: The user who created the page.
  name: created_by
  type: object
- description: The user who last edited the page.
  name: last_edited_by
  type: object
- description: Whether the page has been archived (trashed).
  name: archived
  type: boolean
- description: Whether the page is in the trash.
  name: in_trash
  type: boolean
- description: Page icon, either an emoji or a file object.
  name: icon
  type: object
- description: Page cover image as a file object, or null if not set.
  name: cover
  type: object
- description: Property values of the page. Keys are property names or IDs, and values are property value objects whose structure depends on the property type.
  name: properties
  type: object
- description: The parent of the page (workspace, page, database, or block).
  name: parent
  type: object
- description: The URL of the page in Notion.
  name: url
  type: string
- description: The public URL of the page if published to the web, otherwise null.
  name: public_url
  type:
  - string
  - 'null'
- description: A unique identifier for the API request that returned this object.
  name: request_id
  type: string
provider_name: Notion
provider_slug: notion
schema_file: json-schema/notion-page-schema.json
slug: notion-page
source_filename: notion-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/json-schema/notion-page-schema.json\",\n  \"title\": \"Notion Page\",\n  \"description\": \"A Page object represents a page in a Notion workspace. Pages can exist as standalone pages in a workspace or as items within a database. Each page has properties (metadata fields) and content composed of blocks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"page\",\n      \"description\": \"Always 'page' for page objects.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the page (UUIDv4).\"\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the page was created, in ISO 8601 format.\"\n    },\n\
  \    \"last_edited_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the page was last edited, in ISO 8601 format.\"\n    },\n    \"created_by\": {\n      \"$ref\": \"#/$defs/PartialUser\",\n      \"description\": \"The user who created the page.\"\n    },\n    \"last_edited_by\": {\n      \"$ref\": \"#/$defs/PartialUser\",\n      \"description\": \"The user who last edited the page.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the page has been archived (trashed).\"\n    },\n    \"in_trash\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the page is in the trash.\"\n    },\n    \"icon\": {\n      \"description\": \"Page icon, either an emoji or a file object.\",\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/Emoji\" },\n        { \"$ref\": \"#/$defs/File\" },\n        { \"type\": \"null\" }\n      ]\n    },\n    \"cover\": {\n      \"description\"\
  : \"Page cover image as a file object, or null if not set.\",\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/File\" },\n        { \"type\": \"null\" }\n      ]\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Property values of the page. Keys are property names or IDs, and values are property value objects whose structure depends on the property type.\",\n      \"additionalProperties\": true\n    },\n    \"parent\": {\n      \"$ref\": \"#/$defs/Parent\",\n      \"description\": \"The parent of the page (workspace, page, database, or block).\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the page in Notion.\"\n    },\n    \"public_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The public URL of the page if published to the web, otherwise null.\"\n    },\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"A unique identifier for the API request that returned this object.\"\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"id\",\n    \"created_time\",\n    \"last_edited_time\",\n    \"created_by\",\n    \"last_edited_by\",\n    \"archived\",\n    \"properties\",\n    \"parent\",\n    \"url\"\n  ],\n  \"$defs\": {\n    \"PartialUser\": {\n      \"type\": \"object\",\n      \"description\": \"A partial user reference containing only the object type and ID.\",\n      \"properties\": {\n        \"object\": {\n          \"type\": \"string\",\n          \"const\": \"user\",\n          \"description\": \"Always 'user'.\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the user.\"\n        }\n      },\n      \"required\": [\"object\", \"id\"]\n    },\n    \"Parent\": {\n      \"type\": \"object\",\n      \"description\": \"The parent of a page. Can be a workspace, another page, a database,\
  \ or a block.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"database_id\", \"page_id\", \"block_id\", \"workspace\"],\n          \"description\": \"The type of parent.\"\n        },\n        \"database_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The ID of the parent database. Present when type is 'database_id'.\"\n        },\n        \"page_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The ID of the parent page. Present when type is 'page_id'.\"\n        },\n        \"block_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The ID of the parent block. Present when type is 'block_id'.\"\n        },\n        \"workspace\": {\n          \"type\": \"boolean\",\n          \"description\": \"Always true when the parent is the workspace.\"\n        }\n      },\n   \
  \   \"required\": [\"type\"]\n    },\n    \"Emoji\": {\n      \"type\": \"object\",\n      \"description\": \"An emoji icon.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"emoji\"\n        },\n        \"emoji\": {\n          \"type\": \"string\",\n          \"description\": \"The emoji character.\"\n        }\n      },\n      \"required\": [\"type\", \"emoji\"]\n    },\n    \"File\": {\n      \"type\": \"object\",\n      \"description\": \"A file object, either hosted by Notion or externally.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"file\", \"external\"],\n          \"description\": \"The hosting type of the file.\"\n        },\n        \"file\": {\n          \"type\": \"object\",\n          \"description\": \"Notion-hosted file details. URLs expire after one hour.\",\n          \"properties\": {\n            \"url\": {\n              \"type\": \"string\",\n     \
  \         \"format\": \"uri\",\n              \"description\": \"The authenticated S3 URL.\"\n            },\n            \"expiry_time\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\",\n              \"description\": \"When the URL expires.\"\n            }\n          }\n        },\n        \"external\": {\n          \"type\": \"object\",\n          \"description\": \"Externally hosted file details.\",\n          \"properties\": {\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The external URL.\"\n            }\n          }\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the file.\"\n        }\n      },\n      \"required\": [\"type\"]\n    },\n    \"RichText\": {\n      \"type\": \"object\",\n      \"description\": \"A rich text element with content, annotations, and optional links.\",\n      \"properties\": {\n\
  \        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"text\", \"mention\", \"equation\"],\n          \"description\": \"The type of rich text.\"\n        },\n        \"text\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"content\": {\n              \"type\": \"string\",\n              \"description\": \"The text content.\"\n            },\n            \"link\": {\n              \"type\": [\"object\", \"null\"],\n              \"properties\": {\n                \"url\": {\n                  \"type\": \"string\",\n                  \"format\": \"uri\"\n                }\n              }\n            }\n          }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"bold\": { \"type\": \"boolean\" },\n            \"italic\": { \"type\": \"boolean\" },\n            \"strikethrough\": { \"type\": \"boolean\" },\n            \"underline\": { \"type\": \"boolean\" },\n  \
  \          \"code\": { \"type\": \"boolean\" },\n            \"color\": { \"type\": \"string\" }\n          }\n        },\n        \"plain_text\": {\n          \"type\": \"string\",\n          \"description\": \"The plain text content without annotations.\"\n        },\n        \"href\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"The URL of any link, or null.\"\n        }\n      },\n      \"required\": [\"type\", \"plain_text\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/json-schema/notion-page-schema.json
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
title: Notion Page
---
