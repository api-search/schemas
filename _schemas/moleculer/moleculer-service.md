---
description: JSON Schema for a Moleculer service definition, including actions, events, methods, lifecycle hooks, and mixins.
layout: schema
name: Moleculer Service Schema
properties_list:
- description: Unique service name.
  name: name
  type: string
- description: Service version (number or string).
  name: version
  type: object
- description: Service settings accessible via this.settings.
  name: settings
  type: object
- description: Custom metadata for the service.
  name: metadata
  type: object
- description: Services that must be available before this service starts.
  name: dependencies
  type: array
- description: Mixin schemas to merge into this service.
  name: mixins
  type: array
- description: Service action definitions.
  name: actions
  type: object
- description: Event handler definitions.
  name: events
  type: object
- description: Private methods available within the service.
  name: methods
  type: object
- description: Service-level action hooks.
  name: hooks
  type: object
- description: 'Lifecycle hook: called when the service starts (function reference).'
  name: started
  type: string
- description: 'Lifecycle hook: called when the service stops (function reference).'
  name: stopped
  type: string
- description: 'Lifecycle hook: called when the service is created (function reference).'
  name: created
  type: string
provider_name: Moleculer
provider_slug: moleculer
schema_file: json-schema/moleculer-service.json
slug: moleculer-service
source_filename: moleculer-service.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/moleculer/json-schema/moleculer-service.json\",\n  \"title\": \"Moleculer Service Schema\",\n  \"description\": \"JSON Schema for a Moleculer service definition, including actions, events, methods, lifecycle hooks, and mixins.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique service name.\"\n    },\n    \"version\": {\n      \"description\": \"Service version (number or string).\",\n      \"oneOf\": [\n        { \"type\": \"integer\" },\n        { \"type\": \"string\" }\n      ]\n    },\n    \"settings\": {\n      \"type\": \"object\",\n      \"description\": \"Service settings accessible via this.settings.\",\n      \"additionalProperties\": true\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Custom metadata for the service.\",\n      \"additionalProperties\"\
  : true\n    },\n    \"dependencies\": {\n      \"type\": \"array\",\n      \"description\": \"Services that must be available before this service starts.\",\n      \"items\": {\n        \"oneOf\": [\n          { \"type\": \"string\" },\n          {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"version\": {\n                \"oneOf\": [\n                  { \"type\": \"integer\" },\n                  { \"type\": \"string\" }\n                ]\n              }\n            },\n            \"required\": [\"name\"]\n          }\n        ]\n      }\n    },\n    \"mixins\": {\n      \"type\": \"array\",\n      \"description\": \"Mixin schemas to merge into this service.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"actions\": {\n      \"type\": \"object\",\n      \"description\": \"Service action definitions.\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n   \
  \       {\n            \"type\": \"object\",\n            \"properties\": {\n              \"params\": {\n                \"type\": \"object\",\n                \"description\": \"Parameter validation schema.\",\n                \"additionalProperties\": true\n              },\n              \"cache\": {\n                \"description\": \"Caching configuration for this action.\",\n                \"oneOf\": [\n                  { \"type\": \"boolean\" },\n                  {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"keys\": {\n                        \"type\": \"array\",\n                        \"items\": { \"type\": \"string\" }\n                      },\n                      \"ttl\": { \"type\": \"integer\" }\n                    },\n                    \"additionalProperties\": true\n                  }\n                ]\n              },\n              \"timeout\": {\n                \"type\": \"integer\",\n     \
  \           \"description\": \"Action timeout in milliseconds.\"\n              },\n              \"retryPolicy\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"enabled\": { \"type\": \"boolean\" },\n                  \"retries\": { \"type\": \"integer\" },\n                  \"delay\": { \"type\": \"integer\" }\n                },\n                \"additionalProperties\": true\n              },\n              \"bulkhead\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"enabled\": { \"type\": \"boolean\" },\n                  \"concurrency\": { \"type\": \"integer\" }\n                },\n                \"additionalProperties\": true\n              },\n              \"circuitBreaker\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"enabled\": { \"type\": \"boolean\" },\n                  \"threshold\": { \"type\": \"number\" }\n      \
  \          },\n                \"additionalProperties\": true\n              },\n              \"hooks\": {\n                \"type\": \"object\",\n                \"description\": \"Before and after hooks for this action.\",\n                \"properties\": {\n                  \"before\": {},\n                  \"after\": {}\n                },\n                \"additionalProperties\": true\n              },\n              \"visibility\": {\n                \"type\": \"string\",\n                \"description\": \"Action visibility.\",\n                \"enum\": [\"published\", \"public\", \"protected\", \"private\"],\n                \"default\": \"published\"\n              },\n              \"rest\": {\n                \"description\": \"REST API gateway mapping.\",\n                \"oneOf\": [\n                  { \"type\": \"string\", \"description\": \"Short form, e.g., GET /users\" },\n                  {\n                    \"type\": \"object\",\n                    \"properties\"\
  : {\n                      \"method\": { \"type\": \"string\", \"enum\": [\"GET\", \"POST\", \"PUT\", \"DELETE\", \"PATCH\"] },\n                      \"path\": { \"type\": \"string\" }\n                    }\n                  }\n                ]\n              }\n            },\n            \"additionalProperties\": true\n          },\n          { \"type\": \"boolean\", \"const\": false, \"description\": \"Set to false to disable an inherited action.\" }\n        ]\n      }\n    },\n    \"events\": {\n      \"type\": \"object\",\n      \"description\": \"Event handler definitions.\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n          {\n            \"type\": \"object\",\n            \"properties\": {\n              \"group\": {\n                \"type\": \"string\",\n                \"description\": \"Event group name.\"\n              },\n              \"params\": {\n                \"type\": \"object\",\n                \"description\": \"Event parameter validation\
  \ schema.\",\n                \"additionalProperties\": true\n              }\n            },\n            \"additionalProperties\": true\n          },\n          { \"type\": \"boolean\" }\n        ]\n      }\n    },\n    \"methods\": {\n      \"type\": \"object\",\n      \"description\": \"Private methods available within the service.\",\n      \"additionalProperties\": true\n    },\n    \"hooks\": {\n      \"type\": \"object\",\n      \"description\": \"Service-level action hooks.\",\n      \"properties\": {\n        \"before\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        },\n        \"after\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        },\n        \"error\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      },\n      \"additionalProperties\": true\n    },\n    \"started\": {\n      \"type\": \"string\",\n      \"description\": \"Lifecycle hook: called when\
  \ the service starts (function reference).\"\n    },\n    \"stopped\": {\n      \"type\": \"string\",\n      \"description\": \"Lifecycle hook: called when the service stops (function reference).\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"Lifecycle hook: called when the service is created (function reference).\"\n    }\n  },\n  \"required\": [\"name\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/moleculer/refs/heads/main/json-schema/moleculer-service.json
tags:
- Fault Tolerance
- Frameworks
- JavaScript
- Load Balancing
- Microservices
- Node.js
- Service Discovery
title: Moleculer Service Schema
---
