---
description: Custom events emitted by the rapi-doc web component that can be listened to for integration with application logic.
layout: schema
name: RapiDoc Events
properties_list:
- description: Fired when the OpenAPI spec is successfully parsed and loaded.
  name: spec-loaded
  type: object
- description: Fired before a Try It request is sent. Can be used to modify the request.
  name: before-try
  type: object
- description: Fired after a Try It request completes. Contains the response data.
  name: after-try
  type: object
- description: Fired when the user selects a different API server from the server list.
  name: api-server-change
  type: object
- description: Fired before the component renders the spec. Can be used to modify the spec before display.
  name: before-render
  type: object
provider_name: RapiDoc
provider_slug: rapidoc
schema_file: json-schema/rapidoc-events.json
slug: rapidoc-events
source_filename: rapidoc-events.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/rapidoc/blob/main/json-schema/rapidoc-events.json\",\n  \"title\": \"RapiDoc Events\",\n  \"description\": \"Custom events emitted by the rapi-doc web component that can be listened to for integration with application logic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"spec-loaded\": {\n      \"type\": \"object\",\n      \"description\": \"Fired when the OpenAPI spec is successfully parsed and loaded.\",\n      \"properties\": {\n        \"detail\": {\n          \"type\": \"object\",\n          \"description\": \"The parsed OpenAPI specification object.\"\n        }\n      }\n    },\n    \"before-try\": {\n      \"type\": \"object\",\n      \"description\": \"Fired before a Try It request is sent. Can be used to modify the request.\",\n      \"properties\": {\n        \"detail\": {\n          \"type\": \"object\",\n          \"description\": \"Request\
  \ details including URL, method, headers, and body.\"\n        }\n      }\n    },\n    \"after-try\": {\n      \"type\": \"object\",\n      \"description\": \"Fired after a Try It request completes. Contains the response data.\",\n      \"properties\": {\n        \"detail\": {\n          \"type\": \"object\",\n          \"description\": \"Response details including status, headers, and body.\"\n        }\n      }\n    },\n    \"api-server-change\": {\n      \"type\": \"object\",\n      \"description\": \"Fired when the user selects a different API server from the server list.\",\n      \"properties\": {\n        \"detail\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"selectedServer\": {\n              \"type\": \"object\",\n              \"description\": \"The newly selected server object from the spec.\"\n            }\n          }\n        }\n      }\n    },\n    \"before-render\": {\n      \"type\": \"object\",\n      \"description\": \"Fired before\
  \ the component renders the spec. Can be used to modify the spec before display.\",\n      \"properties\": {\n        \"detail\": {\n          \"type\": \"object\",\n          \"description\": \"The spec data about to be rendered.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rapidoc/refs/heads/main/json-schema/rapidoc-events.json
tags:
- Documentation
- Platform
- Web Components
- OpenAPI
title: RapiDoc Events
---
