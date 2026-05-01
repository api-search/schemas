---
description: Represents a store menu on the DoorDash marketplace, including categories, items, option groups, and modifiers.
layout: schema
name: DoorDash Menu
properties_list:
- description: The merchant-supplied store identifier.
  name: store_id
  type: string
- description: The unique identifier for the menu assigned by DoorDash.
  name: menu_id
  type: string
- description: The menu categories containing items.
  name: categories
  type: array
- description: When the menu was last updated.
  name: last_updated
  type: string
provider_name: doordash
provider_slug: doordash
schema_file: json-schema/doordash-menu-schema.json
slug: doordash-menu
source_filename: doordash-menu-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.doordash.com/schemas/doordash/menu.json\",\n  \"title\": \"DoorDash Menu\",\n  \"description\": \"Represents a store menu on the DoorDash marketplace, including categories, items, option groups, and modifiers.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"store_id\",\n    \"categories\"\n  ],\n  \"properties\": {\n    \"store_id\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant-supplied store identifier.\"\n    },\n    \"menu_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the menu assigned by DoorDash.\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"description\": \"The menu categories containing items.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/Category\"\n      }\n    },\n    \"last_updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"When the menu was last updated.\"\n    }\n  },\n  \"$defs\": {\n    \"Category\": {\n      \"type\": \"object\",\n      \"description\": \"A category grouping related menu items.\",\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"items\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for this category.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the category.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the category.\"\n        },\n        \"sort_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The sort order for this category.\",\n          \"minimum\": 0\n        },\n        \"items\": {\n          \"type\": \"array\",\n          \"description\": \"The items in this category.\"\
  ,\n          \"items\": {\n            \"$ref\": \"#/$defs/MenuItem\"\n          }\n        }\n      }\n    },\n    \"MenuItem\": {\n      \"type\": \"object\",\n      \"description\": \"A menu item available for ordering.\",\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"price\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The merchant-supplied item identifier.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the item.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the item.\"\n        },\n        \"price\": {\n          \"type\": \"integer\",\n          \"description\": \"The item price in cents.\",\n          \"minimum\": 0\n        },\n        \"image_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\"\
  : \"A URL to an image of the item.\"\n        },\n        \"is_active\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the item is currently available for ordering.\"\n        },\n        \"sort_id\": {\n          \"type\": \"integer\",\n          \"description\": \"The sort order for this item within its category.\",\n          \"minimum\": 0\n        },\n        \"option_groups\": {\n          \"type\": \"array\",\n          \"description\": \"Option groups (modifiers) for this item.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/OptionGroup\"\n          }\n        }\n      }\n    },\n    \"OptionGroup\": {\n      \"type\": \"object\",\n      \"description\": \"A group of selectable options or modifiers for a menu item.\",\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"options\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for this\
  \ option group.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the option group.\"\n        },\n        \"min_selections\": {\n          \"type\": \"integer\",\n          \"description\": \"The minimum number of options that must be selected.\",\n          \"minimum\": 0\n        },\n        \"max_selections\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of options that can be selected.\",\n          \"minimum\": 1\n        },\n        \"options\": {\n          \"type\": \"array\",\n          \"description\": \"The available options in this group.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/MenuOption\"\n          }\n        }\n      }\n    },\n    \"MenuOption\": {\n      \"type\": \"object\",\n      \"description\": \"An individual option or modifier within an option group.\",\n      \"required\": [\n        \"id\",\n        \"name\",\n        \"price\"\n  \
  \    ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique identifier for this option.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name of the option.\"\n        },\n        \"price\": {\n          \"type\": \"integer\",\n          \"description\": \"The additional price for this option in cents.\",\n          \"minimum\": 0\n        },\n        \"is_active\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the option is currently available.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/doordash/refs/heads/main/json-schema/doordash-menu-schema.json
tags: []
title: DoorDash Menu
---
