---
description: A Database object represents a database in Notion. Databases are collections of pages organized with a shared schema of properties that define the columns and their types. Databases support filtering, sorting, and querying through the API.
layout: schema
name: Notion Database
properties_list:
- description: Always 'database' for database objects.
  name: object
  type: string
- description: Unique identifier for the database (UUIDv4).
  name: id
  type: string
- description: Date and time when the database was created, in ISO 8601 format.
  name: created_time
  type: string
- description: Date and time when the database was last edited, in ISO 8601 format.
  name: last_edited_time
  type: string
- description: The user who created the database.
  name: created_by
  type: object
- description: The user who last edited the database.
  name: last_edited_by
  type: object
- description: Title of the database as an array of rich text objects.
  name: title
  type: array
- description: Description of the database as an array of rich text objects.
  name: description
  type: array
- description: Database icon, either an emoji or a file.
  name: icon
  type: object
- description: Database cover image, or null if not set.
  name: cover
  type: object
- description: Schema of database properties. Keys are property names, values are property schema objects defining the type and configuration of each column.
  name: properties
  type: object
- description: The parent of the database (workspace or page).
  name: parent
  type: object
- description: The URL of the database in Notion.
  name: url
  type: string
- description: The public URL of the database if published to the web, otherwise null.
  name: public_url
  type:
  - string
  - 'null'
- description: Whether the database has been archived.
  name: archived
  type: boolean
- description: Whether the database is in the trash.
  name: in_trash
  type: boolean
- description: Whether the database appears inline within its parent page rather than as a full page.
  name: is_inline
  type: boolean
- description: A unique identifier for the API request that returned this object.
  name: request_id
  type: string
provider_name: Notion
provider_slug: notion
schema_file: json-schema/notion-database-schema.json
slug: notion-database
source_filename: notion-database-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/json-schema/notion-database-schema.json\",\n  \"title\": \"Notion Database\",\n  \"description\": \"A Database object represents a database in Notion. Databases are collections of pages organized with a shared schema of properties that define the columns and their types. Databases support filtering, sorting, and querying through the API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"object\": {\n      \"type\": \"string\",\n      \"const\": \"database\",\n      \"description\": \"Always 'database' for database objects.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the database (UUIDv4).\"\n    },\n    \"created_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the\
  \ database was created, in ISO 8601 format.\"\n    },\n    \"last_edited_time\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when the database was last edited, in ISO 8601 format.\"\n    },\n    \"created_by\": {\n      \"$ref\": \"#/$defs/PartialUser\",\n      \"description\": \"The user who created the database.\"\n    },\n    \"last_edited_by\": {\n      \"$ref\": \"#/$defs/PartialUser\",\n      \"description\": \"The user who last edited the database.\"\n    },\n    \"title\": {\n      \"type\": \"array\",\n      \"description\": \"Title of the database as an array of rich text objects.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RichText\"\n      }\n    },\n    \"description\": {\n      \"type\": \"array\",\n      \"description\": \"Description of the database as an array of rich text objects.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RichText\"\n      }\n    },\n    \"icon\": {\n      \"description\":\
  \ \"Database icon, either an emoji or a file.\",\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/Emoji\" },\n        { \"$ref\": \"#/$defs/File\" },\n        { \"type\": \"null\" }\n      ]\n    },\n    \"cover\": {\n      \"description\": \"Database cover image, or null if not set.\",\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/File\" },\n        { \"type\": \"null\" }\n      ]\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Schema of database properties. Keys are property names, values are property schema objects defining the type and configuration of each column.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/PropertySchema\"\n      }\n    },\n    \"parent\": {\n      \"$ref\": \"#/$defs/Parent\",\n      \"description\": \"The parent of the database (workspace or page).\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the database in Notion.\"\n\
  \    },\n    \"public_url\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"The public URL of the database if published to the web, otherwise null.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the database has been archived.\"\n    },\n    \"in_trash\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the database is in the trash.\"\n    },\n    \"is_inline\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the database appears inline within its parent page rather than as a full page.\"\n    },\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the API request that returned this object.\"\n    }\n  },\n  \"required\": [\n    \"object\",\n    \"id\",\n    \"created_time\",\n    \"last_edited_time\",\n    \"created_by\",\n    \"last_edited_by\",\n    \"title\",\n    \"description\",\n    \"properties\",\n\
  \    \"parent\",\n    \"url\",\n    \"archived\"\n  ],\n  \"$defs\": {\n    \"PartialUser\": {\n      \"type\": \"object\",\n      \"description\": \"A partial user reference containing only the object type and ID.\",\n      \"properties\": {\n        \"object\": {\n          \"type\": \"string\",\n          \"const\": \"user\",\n          \"description\": \"Always 'user'.\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique identifier for the user.\"\n        }\n      },\n      \"required\": [\"object\", \"id\"]\n    },\n    \"Parent\": {\n      \"type\": \"object\",\n      \"description\": \"The parent of a database. Can be a workspace or a page.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"database_id\", \"page_id\", \"block_id\", \"workspace\"],\n          \"description\": \"The type of parent.\"\n        },\n        \"database_id\": {\n  \
  \        \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"page_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"block_id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\"\n        },\n        \"workspace\": {\n          \"type\": \"boolean\"\n        }\n      },\n      \"required\": [\"type\"]\n    },\n    \"PropertySchema\": {\n      \"type\": \"object\",\n      \"description\": \"Defines a database property's type and configuration. The type field determines which type-specific configuration object is present.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the property.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the property (column name).\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The description\
  \ of the property.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of property.\",\n          \"enum\": [\n            \"title\",\n            \"rich_text\",\n            \"number\",\n            \"select\",\n            \"multi_select\",\n            \"date\",\n            \"people\",\n            \"files\",\n            \"checkbox\",\n            \"url\",\n            \"email\",\n            \"phone_number\",\n            \"formula\",\n            \"relation\",\n            \"rollup\",\n            \"created_time\",\n            \"created_by\",\n            \"last_edited_time\",\n            \"last_edited_by\",\n            \"status\",\n            \"unique_id\",\n            \"verification\"\n          ]\n        },\n        \"title\": {\n          \"type\": \"object\",\n          \"description\": \"Title property configuration (empty object).\"\n        },\n        \"rich_text\": {\n          \"type\": \"object\",\n       \
  \   \"description\": \"Rich text property configuration (empty object).\"\n        },\n        \"number\": {\n          \"type\": \"object\",\n          \"description\": \"Number property configuration.\",\n          \"properties\": {\n            \"format\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"number\",\n                \"number_with_commas\",\n                \"percent\",\n                \"dollar\",\n                \"canadian_dollar\",\n                \"euro\",\n                \"pound\",\n                \"yen\",\n                \"ruble\",\n                \"rupee\",\n                \"won\",\n                \"yuan\",\n                \"real\",\n                \"lira\",\n                \"rupiah\",\n                \"franc\",\n                \"hong_kong_dollar\",\n                \"new_zealand_dollar\",\n                \"krona\",\n                \"norwegian_krone\",\n                \"mexican_peso\",\n                \"rand\"\
  ,\n                \"new_taiwan_dollar\",\n                \"danish_krone\",\n                \"zloty\",\n                \"baht\",\n                \"forint\",\n                \"koruna\",\n                \"shekel\",\n                \"chilean_peso\",\n                \"philippine_peso\",\n                \"dirham\",\n                \"colombian_peso\",\n                \"riyal\",\n                \"ringgit\",\n                \"leu\",\n                \"argentine_peso\",\n                \"uruguayan_peso\",\n                \"singapore_dollar\"\n              ]\n            }\n          }\n        },\n        \"select\": {\n          \"type\": \"object\",\n          \"description\": \"Select property configuration.\",\n          \"properties\": {\n            \"options\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/$defs/SelectOption\"\n              }\n            }\n          }\n        },\n        \"multi_select\": {\n        \
  \  \"type\": \"object\",\n          \"description\": \"Multi-select property configuration.\",\n          \"properties\": {\n            \"options\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/$defs/SelectOption\"\n              }\n            }\n          }\n        },\n        \"status\": {\n          \"type\": \"object\",\n          \"description\": \"Status property configuration.\",\n          \"properties\": {\n            \"options\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/$defs/SelectOption\"\n              }\n            },\n            \"groups\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": { \"type\": \"string\" },\n                  \"name\": { \"type\": \"string\" },\n                  \"color\": { \"type\": \"string\" },\n                  \"\
  option_ids\": {\n                    \"type\": \"array\",\n                    \"items\": { \"type\": \"string\" }\n                  }\n                }\n              }\n            }\n          }\n        },\n        \"formula\": {\n          \"type\": \"object\",\n          \"description\": \"Formula property configuration.\",\n          \"properties\": {\n            \"expression\": {\n              \"type\": \"string\",\n              \"description\": \"The formula expression.\"\n            }\n          }\n        },\n        \"relation\": {\n          \"type\": \"object\",\n          \"description\": \"Relation property configuration.\",\n          \"properties\": {\n            \"database_id\": {\n              \"type\": \"string\",\n              \"format\": \"uuid\",\n              \"description\": \"The ID of the related database.\"\n            },\n            \"type\": {\n              \"type\": \"string\",\n              \"enum\": [\"single_property\", \"dual_property\"\
  ]\n            },\n            \"single_property\": {\n              \"type\": \"object\"\n            },\n            \"dual_property\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"synced_property_name\": { \"type\": \"string\" },\n                \"synced_property_id\": { \"type\": \"string\" }\n              }\n            }\n          }\n        },\n        \"rollup\": {\n          \"type\": \"object\",\n          \"description\": \"Rollup property configuration.\",\n          \"properties\": {\n            \"relation_property_name\": { \"type\": \"string\" },\n            \"relation_property_id\": { \"type\": \"string\" },\n            \"rollup_property_name\": { \"type\": \"string\" },\n            \"rollup_property_id\": { \"type\": \"string\" },\n            \"function\": {\n              \"type\": \"string\",\n              \"enum\": [\n                \"count\",\n                \"count_values\",\n                \"empty\",\n   \
  \             \"not_empty\",\n                \"unique\",\n                \"show_unique\",\n                \"percent_empty\",\n                \"percent_not_empty\",\n                \"sum\",\n                \"average\",\n                \"median\",\n                \"min\",\n                \"max\",\n                \"range\",\n                \"earliest_date\",\n                \"latest_date\",\n                \"date_range\",\n                \"checked\",\n                \"unchecked\",\n                \"percent_checked\",\n                \"percent_unchecked\",\n                \"count_per_group\",\n                \"show_original\"\n              ]\n            }\n          }\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"SelectOption\": {\n      \"type\": \"object\",\n      \"description\": \"A select or multi-select option.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the option.\"\
  \n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the option.\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"The color of the option.\",\n          \"enum\": [\n            \"default\",\n            \"gray\",\n            \"brown\",\n            \"orange\",\n            \"yellow\",\n            \"green\",\n            \"blue\",\n            \"purple\",\n            \"pink\",\n            \"red\"\n          ]\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The description of the option.\"\n        }\n      }\n    },\n    \"Emoji\": {\n      \"type\": \"object\",\n      \"description\": \"An emoji icon.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"emoji\"\n        },\n        \"emoji\": {\n          \"type\": \"string\",\n          \"description\": \"The emoji character.\"\
  \n        }\n      },\n      \"required\": [\"type\", \"emoji\"]\n    },\n    \"File\": {\n      \"type\": \"object\",\n      \"description\": \"A file object, either Notion-hosted or external.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"file\", \"external\"]\n        },\n        \"file\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            },\n            \"expiry_time\": {\n              \"type\": \"string\",\n              \"format\": \"date-time\"\n            }\n          }\n        },\n        \"external\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\"\
  type\"]\n    },\n    \"RichText\": {\n      \"type\": \"object\",\n      \"description\": \"A rich text element.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"text\", \"mention\", \"equation\"]\n        },\n        \"text\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"content\": { \"type\": \"string\" },\n            \"link\": {\n              \"type\": [\"object\", \"null\"],\n              \"properties\": {\n                \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n              }\n            }\n          }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"bold\": { \"type\": \"boolean\" },\n            \"italic\": { \"type\": \"boolean\" },\n            \"strikethrough\": { \"type\": \"boolean\" },\n            \"underline\": { \"type\": \"boolean\" },\n            \"code\": { \"type\": \"boolean\" },\n     \
  \       \"color\": { \"type\": \"string\" }\n          }\n        },\n        \"plain_text\": { \"type\": \"string\" },\n        \"href\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\"type\", \"plain_text\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/notion/refs/heads/main/json-schema/notion-database-schema.json
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
title: Notion Database
---
