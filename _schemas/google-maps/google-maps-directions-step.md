---
description: A single step of a route leg
layout: schema
name: Step
properties_list:
- description: Formatted instructions for this step, presented as an HTML text string.
  name: html_instructions
  type: string
- description: The travel mode for this step
  name: travel_mode
  type: string
- description: The maneuver action for this step (e.g., turn-left, roundabout-right, merge, straight, etc.).
  name: maneuver
  type: string
- description: Sub-steps for walking or transit legs in multi-modal routes
  name: steps
  type: array
provider_name: Google Maps Platform
provider_slug: google-maps
schema_file: json-schema/google-maps-directions-step-schema.json
slug: google-maps-directions-step
source_filename: google-maps-directions-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Step\",\n  \"type\": \"object\",\n  \"description\": \"A single step of a route leg\",\n  \"properties\": {\n    \"html_instructions\": {\n      \"type\": \"string\",\n      \"description\": \"Formatted instructions for this step, presented as an HTML text string.\"\n    },\n    \"travel_mode\": {\n      \"type\": \"string\",\n      \"description\": \"The travel mode for this step\"\n    },\n    \"maneuver\": {\n      \"type\": \"string\",\n      \"description\": \"The maneuver action for this step (e.g., turn-left, roundabout-right, merge, straight, etc.).\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Sub-steps for walking or transit legs in multi-modal routes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-maps/refs/heads/main/json-schema/google-maps-directions-step-schema.json
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
title: Step
---
