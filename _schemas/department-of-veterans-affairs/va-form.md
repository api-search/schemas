---
description: An official Department of Veterans Affairs form catalog entry.
layout: schema
name: VA Form
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Department of Veterans Affairs (VA)
provider_slug: department-of-veterans-affairs
schema_file: json-schema/va-form-schema.json
slug: va-form
source_filename: va-form-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-veterans-affairs/schemas/form.json\",\n  \"title\": \"VA Form\",\n  \"description\": \"An official Department of Veterans Affairs form catalog entry.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"attributes\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\" },\n    \"type\": { \"type\": \"string\", \"const\": \"va_form\" },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"required\": [\"formName\", \"url\", \"title\"],\n      \"properties\": {\n        \"formName\": { \"type\": \"string\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"title\": { \"type\": \"string\" },\n        \"firstIssuedOn\": { \"type\": [\"string\", \"null\"], \"format\": \"date\" },\n        \"lastRevisionOn\": { \"type\": [\"string\", \"null\"], \"format\": \"date\" },\n        \"pages\": { \"type\": \"integer\"\
  , \"minimum\": 0 },\n        \"sha256\": { \"type\": [\"string\", \"null\"] },\n        \"validPdf\": { \"type\": \"boolean\" },\n        \"formUsage\": { \"type\": [\"string\", \"null\"] },\n        \"formToolIntro\": { \"type\": [\"string\", \"null\"] },\n        \"formToolUrl\": { \"type\": [\"string\", \"null\"], \"format\": \"uri\" },\n        \"formType\": { \"type\": [\"string\", \"null\"] },\n        \"language\": { \"type\": \"string\" },\n        \"deletedAt\": { \"type\": [\"string\", \"null\"], \"format\": \"date-time\" },\n        \"relatedForms\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n        \"benefitCategories\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"description\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"vaFormAdministration\": { \"type\": [\"string\", \"null\"\
  ] }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-veterans-affairs/refs/heads/main/json-schema/va-form-schema.json
tags:
- Federal Government
- Healthcare
- Veterans
title: VA Form
---
