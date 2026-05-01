---
description: JSON Schema for Fastify route schema definitions used for request validation and response serialization.
layout: schema
name: Fastify Route Schema Definition
properties_list:
- description: HTTP method(s) for the route.
  name: method
  type: object
- description: Route URL path (e.g., /api/users/:id).
  name: url
  type: string
- description: Schema definitions for request validation and response serialization.
  name: schema
  type: object
- description: Attach validation errors to the request instead of sending 400.
  name: attachValidation
  type: boolean
- description: Automatically create a HEAD route for GET routes.
  name: exposeHeadRoute
  type: boolean
- description: How to handle trailing slashes when a prefix is set.
  name: prefixTrailingSlash
  type: string
- description: Maximum allowed body size for this route in bytes.
  name: bodyLimit
  type: integer
- description: Route-specific log level.
  name: logLevel
  type: string
- description: Custom route-level configuration.
  name: config
  type: object
- description: Custom route constraints (e.g., version, host).
  name: constraints
  type: object
provider_name: Fastify
provider_slug: fastify
schema_file: json-schema/fastify-route-schema.json
slug: fastify-route
source_filename: fastify-route-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/fastify/json-schema/fastify-route-schema.json\",\n  \"title\": \"Fastify Route Schema Definition\",\n  \"description\": \"JSON Schema for Fastify route schema definitions used for request validation and response serialization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"method\": {\n      \"description\": \"HTTP method(s) for the route.\",\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"enum\": [\"GET\", \"POST\", \"PUT\", \"DELETE\", \"PATCH\", \"HEAD\", \"OPTIONS\"]\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"GET\", \"POST\", \"PUT\", \"DELETE\", \"PATCH\", \"HEAD\", \"OPTIONS\"]\n          }\n        }\n      ]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Route URL path (e.g., /api/users/:id).\"\
  \n    },\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"Schema definitions for request validation and response serialization.\",\n      \"properties\": {\n        \"body\": {\n          \"type\": \"object\",\n          \"description\": \"JSON Schema for request body validation.\",\n          \"additionalProperties\": true\n        },\n        \"querystring\": {\n          \"type\": \"object\",\n          \"description\": \"JSON Schema for query string parameter validation.\",\n          \"additionalProperties\": true\n        },\n        \"params\": {\n          \"type\": \"object\",\n          \"description\": \"JSON Schema for URL parameter validation.\",\n          \"additionalProperties\": true\n        },\n        \"headers\": {\n          \"type\": \"object\",\n          \"description\": \"JSON Schema for request header validation.\",\n          \"additionalProperties\": true\n        },\n        \"response\": {\n          \"type\": \"object\",\n      \
  \    \"description\": \"Response schemas keyed by HTTP status code for serialization.\",\n          \"patternProperties\": {\n            \"^[1-5][0-9]{2}$\": {\n              \"type\": \"object\",\n              \"description\": \"JSON Schema for response body at this status code.\",\n              \"additionalProperties\": true\n            },\n            \"^2xx$\": {\n              \"type\": \"object\",\n              \"description\": \"JSON Schema for all 2xx responses.\",\n              \"additionalProperties\": true\n            }\n          },\n          \"additionalProperties\": true\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"description\": \"OpenAPI tags for documentation.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"summary\": {\n          \"type\": \"string\",\n          \"description\": \"OpenAPI summary for the route.\"\n        },\n        \"description\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"OpenAPI description for the route.\"\n        },\n        \"consumes\": {\n          \"type\": \"array\",\n          \"description\": \"Accepted content types.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"produces\": {\n          \"type\": \"array\",\n          \"description\": \"Produced content types.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"security\": {\n          \"type\": \"array\",\n          \"description\": \"OpenAPI security requirements.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"string\" }\n            }\n          }\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"attachValidation\": {\n      \"type\": \"boolean\",\n      \"description\": \"Attach validation errors to the request\
  \ instead of sending 400.\",\n      \"default\": false\n    },\n    \"exposeHeadRoute\": {\n      \"type\": \"boolean\",\n      \"description\": \"Automatically create a HEAD route for GET routes.\",\n      \"default\": true\n    },\n    \"prefixTrailingSlash\": {\n      \"type\": \"string\",\n      \"description\": \"How to handle trailing slashes when a prefix is set.\",\n      \"enum\": [\"slash\", \"no-slash\", \"both\"],\n      \"default\": \"both\"\n    },\n    \"bodyLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum allowed body size for this route in bytes.\"\n    },\n    \"logLevel\": {\n      \"type\": \"string\",\n      \"description\": \"Route-specific log level.\",\n      \"enum\": [\"trace\", \"debug\", \"info\", \"warn\", \"error\", \"fatal\", \"silent\"]\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Custom route-level configuration.\",\n      \"additionalProperties\": true\n    },\n    \"constraints\": {\n    \
  \  \"type\": \"object\",\n      \"description\": \"Custom route constraints (e.g., version, host).\",\n      \"properties\": {\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"Version constraint for content-type versioning.\"\n        },\n        \"host\": {\n          \"type\": \"string\",\n          \"description\": \"Host constraint for virtual hosting.\"\n        }\n      },\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"method\", \"url\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fastify/refs/heads/main/json-schema/fastify-route-schema.json
tags:
- Frameworks
- High Performance
- JavaScript
- JSON Schema
- Node.js
- TypeScript
title: Fastify Route Schema Definition
---
