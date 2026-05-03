---
description: Schema representing a RapidAPI Gateway configuration, including routing rules, authentication, rate limiting, security policies, and deployment settings.
layout: schema
name: RapidAPI Gateway Configuration
properties_list:
- description: Unique identifier for the gateway instance
  name: id
  type: string
- description: Display name for the gateway
  name: name
  type: string
- description: Description of the gateway's purpose and configuration
  name: description
  type: string
- description: How the gateway is deployed within the infrastructure
  name: deploymentModel
  type: string
- description: Current operational status of the gateway
  name: status
  type: string
- description: The base URL where the gateway accepts incoming requests
  name: baseUrl
  type: string
- description: Unique secret added as X-RapidAPI-Proxy-Secret header to verify requests come from Rapid Runtime
  name: proxySecret
  type: string
- description: Routing rules that determine how requests are forwarded to backend services
  name: routes
  type: array
- description: Authentication scheme and configuration for the gateway
  name: authentication
  type: object
- description: Rate limiting policies to control API usage
  name: rateLimiting
  type: object
- description: Security policies including IP filtering and CORS
  name: security
  type: object
- description: Timestamp when the gateway was created
  name: createdAt
  type: string
- description: Timestamp when the gateway was last modified
  name: updatedAt
  type: string
provider_name: RapidAPI
provider_slug: rapidapi
schema_file: json-schema/rapidapi-gateway-config-schema.json
slug: rapidapi-gateway-config
source_filename: rapidapi-gateway-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://rapidapi.com/schemas/rapidapi/gateway-config.json\",\n  \"title\": \"RapidAPI Gateway Configuration\",\n  \"description\": \"Schema representing a RapidAPI Gateway configuration, including routing rules, authentication, rate limiting, security policies, and deployment settings.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the gateway instance\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the gateway\",\n      \"minLength\": 1,\n      \"maxLength\": 200\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the gateway's purpose and configuration\"\n    },\n    \"deploymentModel\": {\n      \"type\": \"string\",\n      \"enum\": [\"cloud\", \"on-premise\", \"hybrid\"\
  ],\n      \"description\": \"How the gateway is deployed within the infrastructure\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"inactive\", \"provisioning\"],\n      \"description\": \"Current operational status of the gateway\"\n    },\n    \"baseUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The base URL where the gateway accepts incoming requests\"\n    },\n    \"proxySecret\": {\n      \"type\": \"string\",\n      \"description\": \"Unique secret added as X-RapidAPI-Proxy-Secret header to verify requests come from Rapid Runtime\"\n    },\n    \"routes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Route\"\n      },\n      \"description\": \"Routing rules that determine how requests are forwarded to backend services\"\n    },\n    \"authentication\": {\n      \"$ref\": \"#/$defs/AuthenticationConfig\",\n      \"description\": \"Authentication scheme and configuration\
  \ for the gateway\"\n    },\n    \"rateLimiting\": {\n      \"$ref\": \"#/$defs/RateLimitConfig\",\n      \"description\": \"Rate limiting policies to control API usage\"\n    },\n    \"security\": {\n      \"$ref\": \"#/$defs/SecurityConfig\",\n      \"description\": \"Security policies including IP filtering and CORS\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the gateway was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the gateway was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"Route\": {\n      \"type\": \"object\",\n      \"required\": [\"pathPattern\", \"targetUrl\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the route\"\n        },\n        \"pathPattern\": {\n          \"type\": \"string\",\n    \
  \      \"description\": \"URL path pattern to match incoming requests, supports wildcards\"\n        },\n        \"targetUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Backend service URL to forward matching requests to\"\n        },\n        \"methods\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"]\n          },\n          \"description\": \"HTTP methods this route handles, empty means all methods\"\n        },\n        \"stripPrefix\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to strip the matched path prefix before forwarding\"\n        },\n        \"priority\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Route priority for matching order, higher values match first\"\n        },\n        \"enabled\": {\n          \"type\": \"\
  boolean\",\n          \"description\": \"Whether this route is currently active\"\n        }\n      },\n      \"description\": \"A routing rule that forwards matching requests to a backend service\"\n    },\n    \"AuthenticationConfig\": {\n      \"type\": \"object\",\n      \"required\": [\"scheme\"],\n      \"properties\": {\n        \"scheme\": {\n          \"type\": \"string\",\n          \"enum\": [\"rapidapi_default\", \"oauth2\", \"header\", \"query\", \"basic\"],\n          \"description\": \"The primary authentication scheme used by the gateway\"\n        },\n        \"requireRapidApiKey\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the X-RapidAPI-Key header is required for all requests\"\n        },\n        \"oauth2Config\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"authorizationUrl\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"OAuth2 authorization\
  \ endpoint URL\"\n            },\n            \"tokenUrl\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"OAuth2 token endpoint URL\"\n            },\n            \"scopes\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Available OAuth2 scopes\"\n            }\n          },\n          \"description\": \"OAuth2 configuration when scheme is oauth2\"\n        },\n        \"headerConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"headerName\": {\n              \"type\": \"string\",\n              \"description\": \"Custom header name for authentication\"\n            }\n          },\n          \"description\": \"Header-based authentication configuration\"\n        }\n      },\n      \"description\": \"Gateway authentication configuration\"\n    },\n    \"RateLimitConfig\": {\n    \
  \  \"type\": \"object\",\n      \"properties\": {\n        \"requestsPerSecond\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Maximum requests per second per consumer\"\n        },\n        \"requestsPerMinute\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Maximum requests per minute per consumer\"\n        },\n        \"requestsPerDay\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Maximum requests per day per consumer\"\n        },\n        \"maxRequestSizeBytes\": {\n          \"type\": \"integer\",\n          \"minimum\": 1024,\n          \"description\": \"Maximum request body size in bytes to prevent misuse\"\n        },\n        \"burstLimit\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Maximum burst of concurrent requests allowed\"\n        }\n      },\n      \"description\": \"Rate limiting\
  \ configuration to protect APIs from overuse\"\n    },\n    \"SecurityConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ipAllowList\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"IP address or CIDR range\"\n          },\n          \"description\": \"List of allowed IP addresses or CIDR ranges\"\n        },\n        \"ipDenyList\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"IP address or CIDR range\"\n          },\n          \"description\": \"List of denied IP addresses or CIDR ranges\"\n        },\n        \"corsEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether CORS is enabled for cross-origin requests\"\n        },\n        \"corsConfig\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"allowedOrigins\": {\n              \"type\": \"\
  array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Allowed CORS origins\"\n            },\n            \"allowedMethods\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Allowed HTTP methods for CORS preflight\"\n            },\n            \"allowedHeaders\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"Allowed request headers for CORS\"\n            },\n            \"maxAge\": {\n              \"type\": \"integer\",\n              \"minimum\": 0,\n              \"description\": \"CORS preflight response cache duration in seconds\"\n            }\n          },\n          \"description\": \"CORS configuration details\"\n        },\n        \"validateProxySecret\": {\n          \"type\": \"boolean\"\
  ,\n          \"description\": \"Whether to validate the X-RapidAPI-Proxy-Secret header on incoming requests\"\n        }\n      },\n      \"description\": \"Security policies for the gateway\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/json-schema/rapidapi-gateway-config-schema.json
tags:
- API Marketplace
- API Management
- API Testing
- API Gateway
- API Design
- Enterprise
title: RapidAPI Gateway Configuration
---
