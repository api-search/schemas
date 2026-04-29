---
description: deck dimensions are used as a reference to display the entire aircraft or to the section associated to the requested cabin (or set of cabins)
layout: schema
name: DeckConfiguration
properties_list:
- description: Width (y-axis) of the deck.
  name: width
  type: integer
- description: Length (x-axis) of the deck.
  name: length
  type: integer
- description: seat row where the deck is starting
  name: startSeatRow
  type: integer
- description: seat row where the deck is ending
  name: endSeatRow
  type: integer
- description: Start x coordinate of the wings.The wings display starts relatively to the length.
  name: startWingsX
  type: integer
- description: End x coordinate of the wings.The wings display ends relatively to the length.
  name: endWingsX
  type: integer
- description: seat row where the wing is starting
  name: startWingsRow
  type: integer
- description: seat row where the wing is ending
  name: endWingsRow
  type: integer
- description: X coordinate of the exit rows.The exit rows are displayed relatively to the length.
  name: exitRowsX
  type: array
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/seatmap-display-deckconfiguration-schema.json
slug: seatmap-display-deckconfiguration
source_filename: seatmap-display-deckconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DeckConfiguration\",\n  \"description\": \"deck dimensions are used as a reference to display the entire aircraft or to the section associated to the requested cabin (or set of cabins)\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Width (y-axis) of the deck.\"\n    },\n    \"length\": {\n      \"type\": \"integer\",\n      \"description\": \"Length (x-axis) of the deck.\"\n    },\n    \"startSeatRow\": {\n      \"type\": \"integer\",\n      \"description\": \"seat row where the deck is starting\"\n    },\n    \"endSeatRow\": {\n      \"type\": \"integer\",\n      \"description\": \"seat row where the deck is ending\"\n    },\n    \"startWingsX\": {\n      \"type\": \"integer\",\n      \"description\": \"Start x coordinate of the wings.The wings display starts relatively to the length.\"\n    },\n    \"endWingsX\": {\n  \
  \    \"type\": \"integer\",\n      \"description\": \"End x coordinate of the wings.The wings display ends relatively to the length.\"\n    },\n    \"startWingsRow\": {\n      \"type\": \"integer\",\n      \"description\": \"seat row where the wing is starting\"\n    },\n    \"endWingsRow\": {\n      \"type\": \"integer\",\n      \"description\": \"seat row where the wing is ending\"\n    },\n    \"exitRowsX\": {\n      \"type\": \"array\",\n      \"description\": \"X coordinate of the exit rows.The exit rows are displayed relatively to the length.\",\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/seatmap-display-deckconfiguration-schema.json
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: DeckConfiguration
---
