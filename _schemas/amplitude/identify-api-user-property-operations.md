---
description: An object containing user property operations. Each key is an operation type and the value is an object of property names to values.
layout: schema
name: UserPropertyOperations
properties_list:
- description: Set the value of a user property. If the property already exists, the value is overwritten.
  name: $set
  type: object
- description: Set the value of a user property only if it has not already been set. Useful for properties like initial_referrer.
  name: $setOnce
  type: object
- description: Increment a numeric user property by the specified value.
  name: $add
  type: object
- description: Append a value or values to a list user property.
  name: $append
  type: object
- description: Prepend a value or values to a list user property.
  name: $prepend
  type: object
- description: Remove a user property by setting its value to the string $unset.
  name: $unset
  type: object
- description: Remove a value from a list user property.
  name: $remove
  type: object
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/identify-api-user-property-operations-schema.json
slug: identify-api-user-property-operations
source_filename: identify-api-user-property-operations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/identify-api-user-property-operations-schema.json\",\n  \"title\": \"UserPropertyOperations\",\n  \"description\": \"An object containing user property operations. Each key is an operation type and the value is an object of property names to values.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"$set\": {\n      \"type\": \"object\",\n      \"description\": \"Set the value of a user property. If the property already exists, the value is overwritten.\",\n      \"additionalProperties\": true\n    },\n    \"$setOnce\": {\n      \"type\": \"object\",\n      \"description\": \"Set the value of a user property only if it has not already been set. Useful for properties like initial_referrer.\",\n      \"additionalProperties\": true\n    },\n    \"$add\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Increment a numeric user property by the specified value.\",\n      \"additionalProperties\": {\n        \"type\": \"number\"\n      }\n    },\n    \"$append\": {\n      \"type\": \"object\",\n      \"description\": \"Append a value or values to a list user property.\",\n      \"additionalProperties\": true\n    },\n    \"$prepend\": {\n      \"type\": \"object\",\n      \"description\": \"Prepend a value or values to a list user property.\",\n      \"additionalProperties\": true\n    },\n    \"$unset\": {\n      \"type\": \"object\",\n      \"description\": \"Remove a user property by setting its value to the string $unset.\",\n      \"additionalProperties\": true\n    },\n    \"$remove\": {\n      \"type\": \"object\",\n      \"description\": \"Remove a value from a list user property.\",\n      \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/identify-api-user-property-operations-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: UserPropertyOperations
---
