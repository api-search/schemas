---
description: UserProperty schema from Amplitude Taxonomy API
layout: schema
name: UserProperty
properties_list:
- description: The name of the user property.
  name: user_property
  type: string
- description: A description of the user property.
  name: description
  type: string
- description: The data type of the property.
  name: type
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/taxonomy-api-user-property-schema.json
slug: taxonomy-api-user-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-user-property-schema.json\",\n  \"title\": \"UserProperty\",\n  \"description\": \"UserProperty schema from Amplitude Taxonomy API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"user_property\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user property.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the user property.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The data type of the property.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/taxonomy-api-user-property-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserProperty
---
