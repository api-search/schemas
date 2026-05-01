---
description: Schema for a node in the Firebase Realtime Database, representing a JSON tree structure with optional rules and indexing.
layout: schema
name: Firebase Realtime Database Node
properties_list:
- description: Security rule for read access
  name: .read
  type:
  - string
  - boolean
- description: Security rule for write access
  name: .write
  type:
  - string
  - boolean
- description: Validation rule for data written to this node
  name: .validate
  type: string
- description: Child keys to index for ordering and querying
  name: .indexOn
  type: object
provider_name: Google Firebase
provider_slug: google-firebase
schema_file: json-schema/google-firebase-database-node-schema.json
slug: google-firebase-database-node
source_filename: google-firebase-database-node-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://firebase.google.com/schemas/database/node.json\",\n  \"title\": \"Firebase Realtime Database Node\",\n  \"description\": \"Schema for a node in the Firebase Realtime Database, representing a JSON tree structure with optional rules and indexing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \".read\": {\n      \"type\": [\"string\", \"boolean\"],\n      \"description\": \"Security rule for read access\"\n    },\n    \".write\": {\n      \"type\": [\"string\", \"boolean\"],\n      \"description\": \"Security rule for write access\"\n    },\n    \".validate\": {\n      \"type\": \"string\",\n      \"description\": \"Validation rule for data written to this node\"\n    },\n    \".indexOn\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Child keys to index for ordering\
  \ and querying\"\n    }\n  },\n  \"additionalProperties\": {\n    \"$ref\": \"#/$defs/DatabaseValue\"\n  },\n  \"$defs\": {\n    \"DatabaseValue\": {\n      \"description\": \"A value stored in the Firebase Realtime Database\",\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"number\" },\n        { \"type\": \"boolean\" },\n        { \"type\": \"null\" },\n        {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/DatabaseValue\"\n          }\n        }\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-firebase/refs/heads/main/json-schema/google-firebase-database-node-schema.json
tags:
- Analytics
- Authentication
- Backend as a Service
- Cloud Messaging
- Google Cloud
- Hosting
- Mobile
- Real-Time Database
title: Firebase Realtime Database Node
---
