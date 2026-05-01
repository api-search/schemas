---
description: A single food diary entry recorded for a profile on a given date and meal.
layout: schema
name: FatSecret Food Diary Entry
properties_list:
- description: ''
  name: food_entry_id
  type: string
- description: ''
  name: food_entry_name
  type: string
- description: ''
  name: food_id
  type: string
- description: ''
  name: serving_id
  type: string
- description: ''
  name: number_of_units
  type: string
- description: ''
  name: meal
  type: string
- description: Days since the FatSecret epoch (1970-01-01).
  name: date_int
  type: string
- description: ''
  name: calories
  type: string
- description: ''
  name: carbohydrate
  type: string
- description: ''
  name: protein
  type: string
- description: ''
  name: fat
  type: string
provider_name: FatSecret
provider_slug: fatsecret
schema_file: json-schema/fatsecret-food-entry-schema.json
slug: fatsecret-food-entry
source_filename: fatsecret-food-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/json-schema/fatsecret-food-entry-schema.json\",\n  \"title\": \"FatSecret Food Diary Entry\",\n  \"description\": \"A single food diary entry recorded for a profile on a given date and meal.\",\n  \"type\": \"object\",\n  \"required\": [\"food_entry_id\", \"food_id\", \"date_int\", \"meal\"],\n  \"properties\": {\n    \"food_entry_id\": { \"type\": \"string\" },\n    \"food_entry_name\": { \"type\": \"string\" },\n    \"food_id\": { \"type\": \"string\" },\n    \"serving_id\": { \"type\": \"string\" },\n    \"number_of_units\": { \"type\": \"string\" },\n    \"meal\": {\n      \"type\": \"string\",\n      \"enum\": [\"breakfast\", \"lunch\", \"dinner\", \"other\"]\n    },\n    \"date_int\": {\n      \"type\": \"string\",\n      \"description\": \"Days since the FatSecret epoch (1970-01-01).\"\n    },\n    \"calories\":\
  \ { \"type\": \"string\" },\n    \"carbohydrate\": { \"type\": \"string\" },\n    \"protein\": { \"type\": \"string\" },\n    \"fat\": { \"type\": \"string\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/json-schema/fatsecret-food-entry-schema.json
tags:
- Barcode Scanning
- Calories
- Diets
- Exercise
- Fitness
- Food Diary
- Health
- Macronutrients
- Nutrition
- Recipes
- Weight Tracking
title: FatSecret Food Diary Entry
---
