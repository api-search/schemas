---
description: A user in FullStory representing an individual whose sessions, events, and behavioral data are tracked. Users can be anonymous or identified with an external uid.
layout: schema
name: FullStory User
properties_list:
- description: The FullStory-assigned unique identifier for the user
  name: id
  type: string
- description: The external user identifier provided by the integrating system. Omit to create an anonymous user.
  name: uid
  type: string
- description: The display name for the user shown in the FullStory interface
  name: display_name
  type: string
- description: The email address associated with the user
  name: email
  type: string
- description: Custom key-value properties attached to the user profile. In v2, type suffixes are not required as types are inferred automatically.
  name: properties
  type: object
- description: Optional explicit type declarations for custom properties to override default type inference
  name: schema
  type: object
- description: Any type conflicts detected in custom properties where inferred types do not match declared types
  name: type_conflicts
  type: object
- description: URL to view the user profile in the FullStory application
  name: app_url
  type: string
provider_name: FullStory
provider_slug: fullstory
schema_file: json-schema/fullstory-user-schema.json
slug: fullstory-user
source_filename: fullstory-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fullstory.com/schemas/fullstory/user.json\",\n  \"title\": \"FullStory User\",\n  \"description\": \"A user in FullStory representing an individual whose sessions, events, and behavioral data are tracked. Users can be anonymous or identified with an external uid.\",\n  \"type\": \"object\",\n  \"required\": [],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The FullStory-assigned unique identifier for the user\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"The external user identifier provided by the integrating system. Omit to create an anonymous user.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name for the user shown in the FullStory interface\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\"\
  : \"The email address associated with the user\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Custom key-value properties attached to the user profile. In v2, type suffixes are not required as types are inferred automatically.\",\n      \"additionalProperties\": true\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"Optional explicit type declarations for custom properties to override default type inference\",\n      \"additionalProperties\": true\n    },\n    \"type_conflicts\": {\n      \"type\": \"object\",\n      \"description\": \"Any type conflicts detected in custom properties where inferred types do not match declared types\",\n      \"additionalProperties\": true\n    },\n    \"app_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to view the user profile in the FullStory application\"\n    }\n  },\n  \"$defs\": {\n    \"CreateUserRequest\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Request body for creating or updating a user via the Server API\",\n      \"properties\": {\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"External user identifier. Omit to create an anonymous user.\"\n        },\n        \"display_name\": {\n          \"type\": \"string\",\n          \"description\": \"The display name for the user\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address for the user\"\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"description\": \"Custom key-value properties to attach to the user\",\n          \"additionalProperties\": true\n        },\n        \"schema\": {\n          \"type\": \"object\",\n          \"description\": \"Optional explicit type declarations for custom properties\",\n          \"additionalProperties\": true\n        }\n      }\n   \
  \ }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/json-schema/fullstory-user-schema.json
tags:
- Analytics
- Digital Experience
- Session Replay
- Webhooks
- Data Export
title: FullStory User
---
