---
description: A World of Warcraft item
layout: schema
name: WoWItem
properties_list:
- description: Item ID
  name: id
  type: integer
- description: Item name
  name: name
  type: string
- description: Item quality (Common, Rare, Epic, etc.)
  name: quality
  type: object
- description: Item level
  name: level
  type: integer
- description: Item class
  name: item_class
  type: object
- description: Item subclass
  name: item_subclass
  type: object
- description: Inventory type
  name: inventory_type
  type: object
- description: Purchase price in copper
  name: purchase_price
  type: integer
- description: Sell price in copper
  name: sell_price
  type: integer
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-wo-w-item-schema.json
slug: activision-blizzard-wo-w-item
source_filename: activision-blizzard-wo-w-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-item-schema.json\",\n  \"title\": \"WoWItem\",\n  \"description\": \"A World of Warcraft item\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Item ID\",\n      \"example\": 19019\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Item name\",\n      \"example\": \"Thunderfury, Blessed Blade of the Windseeker\"\n    },\n    \"quality\": {\n      \"type\": \"object\",\n      \"description\": \"Item quality (Common, Rare, Epic, etc.)\"\n    },\n    \"level\": {\n      \"type\": \"integer\",\n      \"description\": \"Item level\",\n      \"example\": 80\n    },\n    \"item_class\": {\n      \"type\": \"object\",\n      \"description\": \"Item class\"\n    },\n    \"item_subclass\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Item subclass\"\n    },\n    \"inventory_type\": {\n      \"type\": \"object\",\n      \"description\": \"Inventory type\"\n    },\n    \"purchase_price\": {\n      \"type\": \"integer\",\n      \"description\": \"Purchase price in copper\"\n    },\n    \"sell_price\": {\n      \"type\": \"integer\",\n      \"description\": \"Sell price in copper\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-item-schema.json
tags: []
title: WoWItem
---
