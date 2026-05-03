---
description: Schema representing an OpenAPI document managed in the Scalar Registry, including metadata, registry coordinates, and documentation configuration.
layout: schema
name: Scalar OpenAPI Document Reference
properties_list:
- description: Scalar Registry namespace (org/project format).
  name: namespace
  type: string
- description: Human-readable API title.
  name: title
  type: string
- description: API version string.
  name: version
  type: string
- description: URL to the OpenAPI document (YAML or JSON).
  name: specUrl
  type: string
- description: OpenAPI specification version.
  name: openAPIVersion
  type: string
- description: Whether the registry entry is publicly accessible.
  name: visibility
  type: string
- description: Scalar documentation configuration.
  name: documentation
  type: object
- description: SDK generation configuration for this API.
  name: sdks
  type: array
- description: Spectral rulesets applied to validate this document.
  name: spectralRulesets
  type: array
- description: Classification tags.
  name: tags
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Scalar
provider_slug: scalar
schema_file: json-schema/scalar-openapi-document-schema.json
slug: scalar-openapi-document
source_filename: scalar-openapi-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.com/schemas/scalar/openapi-document\",\n  \"title\": \"Scalar OpenAPI Document Reference\",\n  \"description\": \"Schema representing an OpenAPI document managed in the Scalar Registry, including metadata, registry coordinates, and documentation configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"namespace\", \"title\", \"version\", \"specUrl\"],\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Scalar Registry namespace (org/project format).\",\n      \"pattern\": \"^[a-z0-9-]+/[a-z0-9-]+$\",\n      \"example\": \"my-org/payments-api\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable API title.\",\n      \"example\": \"Payments API\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"API version string.\",\n      \"example\": \"2.1.0\"\n \
  \   },\n    \"specUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the OpenAPI document (YAML or JSON).\"\n    },\n    \"openAPIVersion\": {\n      \"type\": \"string\",\n      \"enum\": [\"3.0.0\", \"3.0.1\", \"3.0.2\", \"3.0.3\", \"3.1.0\"],\n      \"description\": \"OpenAPI specification version.\",\n      \"example\": \"3.1.0\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"Whether the registry entry is publicly accessible.\",\n      \"default\": \"private\"\n    },\n    \"documentation\": {\n      \"type\": \"object\",\n      \"description\": \"Scalar documentation configuration.\",\n      \"properties\": {\n        \"customDomain\": {\n          \"type\": \"string\",\n          \"description\": \"Custom domain for the published docs.\",\n          \"example\": \"api-docs.example.com\"\n        },\n        \"theme\": {\n          \"type\": \"string\"\
  ,\n          \"enum\": [\"default\", \"alternate\", \"moon\", \"purple\", \"solarized\", \"bluePlanet\", \"deepSpace\", \"saturn\", \"kepler\", \"mars\", \"none\"],\n          \"description\": \"Scalar API Reference display theme.\",\n          \"default\": \"default\"\n        },\n        \"darkMode\": {\n          \"type\": \"boolean\",\n          \"description\": \"Enable dark mode by default.\",\n          \"default\": false\n        },\n        \"gitSync\": {\n          \"type\": \"object\",\n          \"description\": \"Git synchronization configuration.\",\n          \"properties\": {\n            \"enabled\": { \"type\": \"boolean\" },\n            \"repository\": {\n              \"type\": \"string\",\n              \"description\": \"GitHub repository in owner/repo format.\"\n            },\n            \"branch\": {\n              \"type\": \"string\",\n              \"description\": \"Branch to sync from.\",\n              \"default\": \"main\"\n            },\n           \
  \ \"specPath\": {\n              \"type\": \"string\",\n              \"description\": \"Path to OpenAPI file in the repository.\"\n            }\n          }\n        }\n      }\n    },\n    \"sdks\": {\n      \"type\": \"array\",\n      \"description\": \"SDK generation configuration for this API.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"language\"],\n        \"properties\": {\n          \"language\": {\n            \"type\": \"string\",\n            \"enum\": [\"typescript\", \"python\", \"go\", \"php\", \"java\", \"ruby\"],\n            \"description\": \"Target programming language.\"\n          },\n          \"packageName\": {\n            \"type\": \"string\",\n            \"description\": \"Package/module name for the generated SDK.\",\n            \"example\": \"payments-client\"\n          },\n          \"githubRepo\": {\n            \"type\": \"string\",\n            \"description\": \"GitHub repository for the generated SDK.\"\n      \
  \    }\n        }\n      }\n    },\n    \"spectralRulesets\": {\n      \"type\": \"array\",\n      \"description\": \"Spectral rulesets applied to validate this document.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Classification tags.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalar/refs/heads/main/json-schema/scalar-openapi-document-schema.json
tags:
- API Client
- API Documentation
- API References
- Code Generation
- Developer Tools
- OpenAPI
- Registry
- SDKs
- Swagger
title: Scalar OpenAPI Document Reference
---
