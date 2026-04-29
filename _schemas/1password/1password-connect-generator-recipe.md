---
description: Configuration for generating a random value for a field, such as password length and character types.
layout: schema
name: GeneratorRecipe
properties_list:
- description: The length of the generated value.
  name: length
  type: integer
- description: The character sets to use when generating the value.
  name: characterSets
  type: array
- description: Characters to exclude from the generated value.
  name: excludeCharacters
  type: string
provider_name: 1Password
provider_slug: 1password
schema_file: json-schema/1password-connect-generator-recipe-schema.json
slug: 1password-connect-generator-recipe
source_filename: 1password-connect-generator-recipe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-generator-recipe-schema.json\",\n  \"title\": \"GeneratorRecipe\",\n  \"description\": \"Configuration for generating a random value for a field, such as password length and character types.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"length\": {\n      \"type\": \"integer\",\n      \"description\": \"The length of the generated value.\",\n      \"minimum\": 1,\n      \"maximum\": 64\n    },\n    \"characterSets\": {\n      \"type\": \"array\",\n      \"description\": \"The character sets to use when generating the value.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"LETTERS\",\n          \"DIGITS\",\n          \"SYMBOLS\"\n        ]\n      }\n    },\n    \"excludeCharacters\": {\n      \"type\": \"string\",\n      \"description\": \"Characters\
  \ to exclude from the generated value.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1password/refs/heads/main/json-schema/1password-connect-generator-recipe-schema.json
tags:
- Password Manager
- Passwords
- Security
- Secrets
title: GeneratorRecipe
---
