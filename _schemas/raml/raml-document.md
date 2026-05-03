---
description: JSON Schema representation of key structural elements in a RAML 1.0 API definition
layout: schema
name: RAML 1.0 Document
properties_list:
- description: The title of the API (required root property)
  name: title
  type: string
- description: The version of the API (e.g., v1, 2.0)
  name: version
  type: string
- description: The base URI for all resources in the API
  name: baseUri
  type: string
- description: Supported protocols
  name: protocols
  type: array
- description: Default media type for request and response bodies
  name: mediaType
  type: object
- description: Overall API description
  name: description
  type: string
- description: User documentation sections
  name: documentation
  type: array
- description: Named data type declarations
  name: types
  type: object
- description: Reusable method-level behaviors
  name: traits
  type: object
- description: Reusable resource patterns
  name: resourceTypes
  type: object
- description: Custom annotation type declarations
  name: annotationTypes
  type: object
- description: Security scheme definitions
  name: securitySchemes
  type: object
- description: External library imports
  name: uses
  type: object
provider_name: RAML
provider_slug: raml
schema_file: json-schema/raml-document-schema.json
slug: raml-document
source_filename: raml-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raml.org/schemas/raml-document\",\n  \"title\": \"RAML 1.0 Document\",\n  \"description\": \"JSON Schema representation of key structural elements in a RAML 1.0 API definition\",\n  \"type\": \"object\",\n  \"required\": [\"title\"],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the API (required root property)\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the API (e.g., v1, 2.0)\"\n    },\n    \"baseUri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The base URI for all resources in the API\"\n    },\n    \"protocols\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"HTTP\", \"HTTPS\"]\n      },\n      \"description\": \"Supported protocols\"\n    },\n    \"mediaType\": {\n   \
  \   \"oneOf\": [\n        { \"type\": \"string\" },\n        {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        }\n      ],\n      \"description\": \"Default media type for request and response bodies\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Overall API description\"\n    },\n    \"documentation\": {\n      \"type\": \"array\",\n      \"description\": \"User documentation sections\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DocumentationItem\"\n      }\n    },\n    \"types\": {\n      \"type\": \"object\",\n      \"description\": \"Named data type declarations\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/TypeDeclaration\"\n      }\n    },\n    \"traits\": {\n      \"type\": \"object\",\n      \"description\": \"Reusable method-level behaviors\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/TraitDeclaration\"\n      }\n    },\n    \"resourceTypes\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Reusable resource patterns\",\n      \"additionalProperties\": {\n        \"type\": \"object\"\n      }\n    },\n    \"annotationTypes\": {\n      \"type\": \"object\",\n      \"description\": \"Custom annotation type declarations\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/AnnotationType\"\n      }\n    },\n    \"securitySchemes\": {\n      \"type\": \"object\",\n      \"description\": \"Security scheme definitions\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/SecurityScheme\"\n      }\n    },\n    \"uses\": {\n      \"type\": \"object\",\n      \"description\": \"External library imports\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"description\": \"Path or URL to a RAML library\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"DocumentationItem\": {\n      \"type\": \"object\",\n      \"required\": [\"title\", \"content\"],\n      \"properties\": {\n    \
  \    \"title\": { \"type\": \"string\" },\n        \"content\": { \"type\": \"string\" }\n      }\n    },\n    \"TypeDeclaration\": {\n      \"type\": \"object\",\n      \"description\": \"A RAML data type declaration\",\n      \"properties\": {\n        \"type\": {\n          \"oneOf\": [\n            { \"type\": \"string\" },\n            { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          ],\n          \"description\": \"Base type or union of types\"\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"description\": \"Object properties (for object types)\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/TypeDeclaration\"\n          }\n        },\n        \"description\": { \"type\": \"string\" },\n        \"required\": { \"type\": \"boolean\" },\n        \"default\": {},\n        \"example\": {},\n        \"examples\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {}\n        },\n\
  \        \"enum\": {\n          \"type\": \"array\",\n          \"description\": \"Allowed enumeration values\"\n        },\n        \"pattern\": {\n          \"type\": \"string\",\n          \"description\": \"Regex pattern for string types\"\n        },\n        \"minLength\": { \"type\": \"integer\" },\n        \"maxLength\": { \"type\": \"integer\" },\n        \"minimum\": { \"type\": \"number\" },\n        \"maximum\": { \"type\": \"number\" }\n      }\n    },\n    \"TraitDeclaration\": {\n      \"type\": \"object\",\n      \"description\": \"A reusable method trait\",\n      \"properties\": {\n        \"description\": { \"type\": \"string\" },\n        \"headers\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/TypeDeclaration\"\n          }\n        },\n        \"queryParameters\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/TypeDeclaration\"\n          }\n\
  \        },\n        \"responses\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/ResponseDeclaration\"\n          }\n        }\n      }\n    },\n    \"ResponseDeclaration\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": { \"type\": \"string\" },\n        \"headers\": {\n          \"type\": \"object\"\n        },\n        \"body\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/TypeDeclaration\"\n          }\n        }\n      }\n    },\n    \"AnnotationType\": {\n      \"type\": \"object\",\n      \"description\": \"A custom annotation type\",\n      \"properties\": {\n        \"type\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" },\n        \"allowedTargets\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"SecurityScheme\": {\n    \
  \  \"type\": \"object\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"OAuth 1.0\", \"OAuth 2.0\", \"Basic Authentication\", \"Digest Authentication\", \"Pass Through\", \"x-other\"]\n        },\n        \"description\": { \"type\": \"string\" },\n        \"displayName\": { \"type\": \"string\" },\n        \"settings\": {\n          \"type\": \"object\",\n          \"description\": \"Type-specific security settings\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/raml/refs/heads/main/json-schema/raml-document-schema.json
tags:
- API Design
- Specification Language
- Standards
- YAML
- REST
- API Modeling
title: RAML 1.0 Document
---
