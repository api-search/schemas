---
description: Schema representing the Redux store configuration and state tree structure used in Redux applications.
layout: schema
name: Redux Store
properties_list:
- description: The current immutable state tree of the application.
  name: state
  type: object
- description: A pure function that takes the current state and an action as arguments and returns a new state result.
  name: reducer
  type: string
- description: Array of middleware functions applied to the store for intercepting actions.
  name: middleware
  type: array
- description: Store enhancers that extend the store with additional capabilities.
  name: enhancers
  type: array
provider_name: Redux
provider_slug: redux
schema_file: json-schema/redux-store-schema.json
slug: redux-store
source_filename: redux-store-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/redux/json-schema/redux-store-schema.json\",\n  \"title\": \"Redux Store\",\n  \"description\": \"Schema representing the Redux store configuration and state tree structure used in Redux applications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"state\": {\n      \"description\": \"The current immutable state tree of the application.\",\n      \"type\": \"object\",\n      \"additionalProperties\": true\n    },\n    \"reducer\": {\n      \"description\": \"A pure function that takes the current state and an action as arguments and returns a new state result.\",\n      \"type\": \"string\",\n      \"examples\": [\"rootReducer\", \"combineReducers({...})\"]\n    },\n    \"middleware\": {\n      \"description\": \"Array of middleware functions applied to the store for intercepting actions.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\":\
  \ \"string\",\n        \"description\": \"Middleware function name\"\n      },\n      \"examples\": [[\"redux-thunk\", \"redux-logger\", \"redux-saga\"]]\n    },\n    \"enhancers\": {\n      \"description\": \"Store enhancers that extend the store with additional capabilities.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\"state\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redux/refs/heads/main/json-schema/redux-store-schema.json
tags:
- Flux Architecture
- Frontend
- Javascript
- Predictable State
- React
- State Management
- Typescript
title: Redux Store
---
