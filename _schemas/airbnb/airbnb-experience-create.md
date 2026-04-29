---
description: ''
layout: schema
name: ExperienceCreate
properties_list:
- description: The display name of the experience.
  name: name
  type: string
- description: The full description of the experience and what guests will do.
  name: description
  type: string
- description: The activity category of the experience.
  name: category
  type: string
- description: ''
  name: location
  type: object
- description: The duration of the experience in minutes.
  name: duration_minutes
  type: integer
- description: The maximum number of guests per session.
  name: max_guests
  type: integer
- description: ''
  name: pricing
  type: object
- description: The languages in which the experience is offered.
  name: languages
  type: array
- description: Items guests should bring to the experience.
  name: what_to_bring
  type: array
- description: Accessibility information for the experience.
  name: accessibility
  type: string
provider_name: airbnb
provider_slug: airbnb
schema_file: json-schema/airbnb-experience-create-schema.json
slug: airbnb-experience-create
source_filename: airbnb-experience-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-create-schema.json\",\n  \"title\": \"ExperienceCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the experience.\",\n      \"maxLength\": 100\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The full description of the experience and what guests will do.\",\n      \"maxLength\": 5000\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The activity category of the experience.\",\n      \"enum\": [\n        \"arts_and_culture\",\n        \"entertainment\",\n        \"food_and_drink\",\n        \"nature_and_outdoors\",\n        \"sports\",\n        \"tours\",\n        \"wellness\"\n      ]\n    },\n    \"location\": {\n      \"$ref\"\
  : \"#/components/schemas/ExperienceLocation\"\n    },\n    \"duration_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The duration of the experience in minutes.\",\n      \"minimum\": 30\n    },\n    \"max_guests\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of guests per session.\",\n      \"minimum\": 1\n    },\n    \"pricing\": {\n      \"$ref\": \"#/components/schemas/ExperiencePricing\"\n    },\n    \"languages\": {\n      \"type\": \"array\",\n      \"description\": \"The languages in which the experience is offered.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"what_to_bring\": {\n      \"type\": \"array\",\n      \"description\": \"Items guests should bring to the experience.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"accessibility\": {\n      \"type\": \"string\",\n      \"description\": \"Accessibility information for the experience.\"\n    }\n  },\n  \"required\"\
  : [\n    \"name\",\n    \"description\",\n    \"category\",\n    \"location\",\n    \"duration_minutes\",\n    \"max_guests\",\n    \"pricing\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/json-schema/airbnb-experience-create-schema.json
tags: []
title: ExperienceCreate
---
