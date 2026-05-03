---
description: An API service definition in TIBCO Mashery, representing a managed API with endpoints, authentication, rate limiting, and traffic management configuration.
layout: schema
name: TIBCO Mashery API Service
properties_list:
- description: Unique identifier for the API service
  name: id
  type: string
- description: API service name
  name: name
  type: string
- description: Description of the API service
  name: description
  type: string
- description: API service version
  name: version
  type: string
- description: Overall queries-per-second rate limit for all endpoints
  name: qpsLimitOverall
  type: integer
- description: Service configuration revision number
  name: revisionNumber
  type: integer
- description: Robots.txt policy for the service
  name: robotsPolicy
  type: string
- description: When the service was created
  name: created
  type: string
- description: When the service was last updated
  name: updated
  type: string
- description: API endpoints defined within the service
  name: endpoints
  type: array
provider_name: TIBCO
provider_slug: tibco
schema_file: json-schema/tibco-api-service-schema.json
slug: tibco-api-service
source_filename: tibco-api-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.tibco.com/schemas/tibco/api-service.json\",\n  \"title\": \"TIBCO Mashery API Service\",\n  \"description\": \"An API service definition in TIBCO Mashery, representing a managed API with endpoints, authentication, rate limiting, and traffic management configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the API service\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"API service name\",\n      \"minLength\": 1\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the API service\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"API service version\"\n    },\n    \"qpsLimitOverall\": {\n      \"type\": \"integer\",\n      \"minimum\"\
  : 0,\n      \"description\": \"Overall queries-per-second rate limit for all endpoints\"\n    },\n    \"revisionNumber\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Service configuration revision number\"\n    },\n    \"robotsPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Robots.txt policy for the service\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the service was created\"\n    },\n    \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the service was last updated\"\n    },\n    \"endpoints\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Endpoint\"\n      },\n      \"description\": \"API endpoints defined within the service\"\n    }\n  },\n  \"$defs\": {\n    \"Endpoint\": {\n      \"type\": \"object\",\n      \"description\": \"An API endpoint within a Mashery\
  \ service, defining the public-facing path, backend system, and security configuration\",\n      \"required\": [\"name\", \"requestAuthenticationType\", \"requestProtocol\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Endpoint unique identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Endpoint display name\"\n        },\n        \"requestAuthenticationType\": {\n          \"type\": \"string\",\n          \"enum\": [\"apiKey\", \"apiKeyAndSecret\", \"oauth\"],\n          \"description\": \"Authentication type required for the endpoint\"\n        },\n        \"requestProtocol\": {\n          \"type\": \"string\",\n          \"enum\": [\"rest\", \"soap\", \"xml-rpc\"],\n          \"description\": \"Request protocol type\"\n        },\n        \"requestPathAlias\": {\n          \"type\": \"string\",\n          \"description\": \"Public path alias for the endpoint\"\n   \
  \     },\n        \"supportedHttpMethods\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"get\", \"post\", \"put\", \"delete\", \"head\", \"patch\", \"options\"]\n          },\n          \"description\": \"HTTP methods supported by this endpoint\"\n        },\n        \"trafficManagerDomain\": {\n          \"type\": \"string\",\n          \"description\": \"Traffic manager domain routing requests\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tibco/refs/heads/main/json-schema/tibco-api-service-schema.json
tags:
- Analytics
- API Management
- Cloud
- Enterprise Software
- Integration
- Messaging
- Real-Time Data
title: TIBCO Mashery API Service
---
