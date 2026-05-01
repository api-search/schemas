---
description: The Locale data structure represents a geographical region or location.
layout: schema
name: Locale
properties_list:
- description: ''
  name: Country
  type: object
- description: ''
  name: Subdivision
  type: object
provider_name: Amazon Mechanical Turk
provider_slug: amazon-mechanical-turk
schema_file: json-schema/amazon-mechanical-turk-locale-schema.json
slug: amazon-mechanical-turk-locale
source_filename: amazon-mechanical-turk-locale-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-locale-schema.json\",\n  \"title\": \"Locale\",\n  \"description\": \"The Locale data structure represents a geographical region or location.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Country\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountryParameters\"\n        },\n        {\n          \"description\": \" The country of the locale. Must be a valid ISO 3166 country code. For example, the code US refers to the United States of America. \"\n        }\n      ]\n    },\n    \"Subdivision\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CountryParameters\"\n        },\n        {\n          \"description\": \"The state or subdivision of the locale. A valid ISO 3166-2 subdivision code. For example,\
  \ the code WA refers to the state of Washington.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Country\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mechanical-turk/refs/heads/main/json-schema/amazon-mechanical-turk-locale-schema.json
tags:
- Crowdsourcing
- Human Intelligence
- Labor
- Machine Learning
- Tasks
title: Locale
---
