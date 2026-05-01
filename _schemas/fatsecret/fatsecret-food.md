---
description: A food item in the FatSecret Platform database, including identification, brand, and per-serving nutrition data.
layout: schema
name: FatSecret Food
properties_list:
- description: Unique identifier for the food.
  name: food_id
  type: string
- description: Display name of the food.
  name: food_name
  type: string
- description: Brand name when food_type is Brand.
  name: brand_name
  type: string
- description: ''
  name: food_type
  type: string
- description: ''
  name: food_url
  type: string
- description: ''
  name: servings
  type: object
provider_name: FatSecret
provider_slug: fatsecret
schema_file: json-schema/fatsecret-food-schema.json
slug: fatsecret-food
source_filename: fatsecret-food-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/json-schema/fatsecret-food-schema.json\",\n  \"title\": \"FatSecret Food\",\n  \"description\": \"A food item in the FatSecret Platform database, including identification, brand, and per-serving nutrition data.\",\n  \"type\": \"object\",\n  \"required\": [\"food_id\", \"food_name\", \"food_type\"],\n  \"properties\": {\n    \"food_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the food.\"\n    },\n    \"food_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the food.\"\n    },\n    \"brand_name\": {\n      \"type\": \"string\",\n      \"description\": \"Brand name when food_type is Brand.\"\n    },\n    \"food_type\": {\n      \"type\": \"string\",\n      \"enum\": [\"Generic\", \"Brand\"]\n    },\n    \"food_url\": {\n      \"type\": \"string\",\n  \
  \    \"format\": \"uri\"\n    },\n    \"servings\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"serving\": {\n          \"oneOf\": [\n            { \"$ref\": \"#/$defs/Serving\" },\n            {\n              \"type\": \"array\",\n              \"items\": { \"$ref\": \"#/$defs/Serving\" }\n            }\n          ]\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"Serving\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"serving_id\": { \"type\": \"string\" },\n        \"serving_description\": { \"type\": \"string\" },\n        \"serving_url\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"metric_serving_amount\": { \"type\": \"string\" },\n        \"metric_serving_unit\": { \"type\": \"string\" },\n        \"calories\": { \"type\": \"string\" },\n        \"carbohydrate\": { \"type\": \"string\" },\n        \"protein\": { \"type\": \"string\" },\n        \"fat\": { \"type\": \"string\" },\n        \"saturated_fat\": { \"type\"\
  : \"string\" },\n        \"polyunsaturated_fat\": { \"type\": \"string\" },\n        \"monounsaturated_fat\": { \"type\": \"string\" },\n        \"trans_fat\": { \"type\": \"string\" },\n        \"cholesterol\": { \"type\": \"string\" },\n        \"sodium\": { \"type\": \"string\" },\n        \"potassium\": { \"type\": \"string\" },\n        \"fiber\": { \"type\": \"string\" },\n        \"sugar\": { \"type\": \"string\" },\n        \"vitamin_a\": { \"type\": \"string\" },\n        \"vitamin_c\": { \"type\": \"string\" },\n        \"calcium\": { \"type\": \"string\" },\n        \"iron\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fatsecret/refs/heads/main/json-schema/fatsecret-food-schema.json
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
title: FatSecret Food
---
