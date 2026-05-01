---
description: A recipe in the FatSecret Platform database, including ingredients, directions, and nutrition.
layout: schema
name: FatSecret Recipe
properties_list:
- description: ''
  name: recipe_id
  type: string
- description: ''
  name: recipe_name
  type: string
- description: ''
  name: recipe_description
  type: string
- description: ''
  name: recipe_url
  type: string
- description: ''
  name: recipe_image
  type: string
- description: ''
  name: number_of_servings
  type: string
- description: ''
  name: preparation_time_min
  type: string
- description: ''
  name: cooking_time_min
  type: string
- description: ''
  name: rating
  type: string
- description: ''
  name: recipe_types
  type: object
- description: ''
  name: ingredients
  type: object
- description: ''
  name: directions
  type: object
- description: ''
  name: serving_sizes
  type: object
provider_name: FatSecret
provider_slug: fatsecret
schema_file: json-schema/fatsecret-recipe-schema.json
slug: fatsecret-recipe
source_filename: fatsecret-recipe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/json-schema/fatsecret-recipe-schema.json\",\n  \"title\": \"FatSecret Recipe\",\n  \"description\": \"A recipe in the FatSecret Platform database, including ingredients, directions, and nutrition.\",\n  \"type\": \"object\",\n  \"required\": [\"recipe_id\", \"recipe_name\"],\n  \"properties\": {\n    \"recipe_id\": { \"type\": \"string\" },\n    \"recipe_name\": { \"type\": \"string\" },\n    \"recipe_description\": { \"type\": \"string\" },\n    \"recipe_url\": { \"type\": \"string\", \"format\": \"uri\" },\n    \"recipe_image\": { \"type\": \"string\", \"format\": \"uri\" },\n    \"number_of_servings\": { \"type\": \"string\" },\n    \"preparation_time_min\": { \"type\": \"string\" },\n    \"cooking_time_min\": { \"type\": \"string\" },\n    \"rating\": { \"type\": \"string\" },\n    \"recipe_types\": {\n      \"type\"\
  : \"object\",\n      \"properties\": {\n        \"recipe_type\": {\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          ]\n        }\n      }\n    },\n    \"ingredients\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ingredient\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"food_id\": { \"type\": \"string\" },\n              \"food_name\": { \"type\": \"string\" },\n              \"ingredient_description\": { \"type\": \"string\" },\n              \"number_of_units\": { \"type\": \"string\" },\n              \"measurement_description\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"directions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"direction\": {\n          \"type\": \"array\",\n          \"items\": {\n \
  \           \"type\": \"object\",\n            \"properties\": {\n              \"direction_number\": { \"type\": \"string\" },\n              \"direction_description\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"serving_sizes\": {\n      \"type\": \"object\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/json-schema/fatsecret-recipe-schema.json
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
title: FatSecret Recipe
---
