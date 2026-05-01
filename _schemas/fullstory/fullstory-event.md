---
description: A custom event in FullStory representing a server-side or client-side action. Events can be associated with sessions and users, and include custom properties for behavioral analysis.
layout: schema
name: FullStory Event
properties_list:
- description: The name of the custom event
  name: name
  type: string
- description: ISO 8601 timestamp for when the event occurred
  name: timestamp
  type: string
- description: Session association for the event
  name: session
  type: object
- description: User association for the event. Not accepted if session.id is provided.
  name: user
  type: object
- description: Custom key-value properties for the event. Supports string, real, integer, boolean, array, and object types. Type suffixes are not required in v2.
  name: properties
  type: object
- description: Optional explicit type declarations for custom event properties
  name: schema
  type: object
provider_name: FullStory
provider_slug: fullstory
schema_file: json-schema/fullstory-event-schema.json
slug: fullstory-event
source_filename: fullstory-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://fullstory.com/schemas/fullstory/event.json\",\n  \"title\": \"FullStory Event\",\n  \"description\": \"A custom event in FullStory representing a server-side or client-side action. Events can be associated with sessions and users, and include custom properties for behavioral analysis.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the custom event\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp for when the event occurred\"\n    },\n    \"session\": {\n      \"$ref\": \"#/$defs/SessionReference\",\n      \"description\": \"Session association for the event\"\n    },\n    \"user\": {\n      \"$ref\": \"#/$defs/UserReference\",\n      \"description\": \"User association for the event.\
  \ Not accepted if session.id is provided.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"description\": \"Custom key-value properties for the event. Supports string, real, integer, boolean, array, and object types. Type suffixes are not required in v2.\",\n      \"additionalProperties\": true\n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"Optional explicit type declarations for custom event properties\",\n      \"additionalProperties\": true\n    }\n  },\n  \"$defs\": {\n    \"SessionReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a session for associating the event with a recorded session\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The session identifier to associate the event with\"\n        },\n        \"use_most_recent\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the most recent session within\
  \ 30 minutes will be used. If no recent session is found and no id is provided, the event is created without a session.\"\n        }\n      }\n    },\n    \"UserReference\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a user for associating the event with a specific user\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The FullStory-assigned user ID\"\n        },\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"The external user identifier\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fullstory/refs/heads/main/json-schema/fullstory-event-schema.json
tags:
- Analytics
- Digital Experience
- Session Replay
- Webhooks
- Data Export
title: FullStory Event
---
