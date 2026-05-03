---
description: JSON Schema for Schemathesis .schemathesis.yml configuration file for configuring property-based API testing.
layout: schema
name: Schemathesis Configuration
properties_list:
- description: URL or file path to the OpenAPI or GraphQL schema to test against.
  name: schema
  type: string
- description: Base URL of the API being tested.
  name: url
  type: string
- description: Number of concurrent workers for parallel test execution.
  name: workers
  type: integer
- description: Maximum allowed response time in milliseconds.
  name: max_response_time
  type: integer
- description: List of checks to perform on responses.
  name: checks
  type: array
- description: Authentication configuration.
  name: auth
  type: object
- description: Additional HTTP headers to include in all requests.
  name: headers
  type: object
- description: Filter test generation to specific endpoint path patterns.
  name: endpoint
  type: object
- description: Filter test generation to specific HTTP methods.
  name: method
  type: object
- description: Filter test generation to operations with specific OpenAPI tags.
  name: tag
  type: object
- description: Maximum number of Hypothesis test examples to generate per operation.
  name: hypothesis_max_examples
  type: integer
- description: Stateful testing mode. 'links' follows OpenAPI Links for multi-step workflow testing.
  name: stateful
  type: string
- description: Whether to sanitize sensitive data in test output and reports.
  name: output_sanitize
  type: boolean
- description: File path for JUnit XML output.
  name: junit_xml
  type: string
provider_name: Schemathesis
provider_slug: schemathesis
schema_file: json-schema/schemathesis-config-schema.json
slug: schemathesis-config
source_filename: schemathesis-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemathesis.io/schema/schemathesis-config-schema.json\",\n  \"title\": \"Schemathesis Configuration\",\n  \"description\": \"JSON Schema for Schemathesis .schemathesis.yml configuration file for configuring property-based API testing.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schema\": {\n      \"type\": \"string\",\n      \"description\": \"URL or file path to the OpenAPI or GraphQL schema to test against.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Base URL of the API being tested.\"\n    },\n    \"workers\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"maximum\": 64,\n      \"default\": 1,\n      \"description\": \"Number of concurrent workers for parallel test execution.\"\n    },\n    \"max_response_time\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\"\
  : \"Maximum allowed response time in milliseconds.\"\n    },\n    \"checks\": {\n      \"type\": \"array\",\n      \"description\": \"List of checks to perform on responses.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"not_a_server_error\",\n          \"status_code_conformance\",\n          \"response_schema_conformance\",\n          \"content_type_conformance\",\n          \"response_headers_conformance\"\n        ]\n      }\n    },\n    \"auth\": {\n      \"type\": \"object\",\n      \"description\": \"Authentication configuration.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"bearer\", \"basic\", \"apikey\", \"oauth2\"]\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"Bearer token or API key value.\"\n        },\n        \"username\": {\n          \"type\": \"string\",\n          \"description\": \"Username for Basic authentication.\"\
  \n        },\n        \"password\": {\n          \"type\": \"string\",\n          \"description\": \"Password for Basic authentication.\"\n        },\n        \"header\": {\n          \"type\": \"string\",\n          \"description\": \"Header name for API key authentication.\"\n        }\n      }\n    },\n    \"headers\": {\n      \"type\": \"object\",\n      \"description\": \"Additional HTTP headers to include in all requests.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"endpoint\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Filter test generation to specific endpoint path patterns.\"\n    },\n    \"method\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Filter test generation to specific HTTP methods.\"\n    },\n    \"\
  tag\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Filter test generation to operations with specific OpenAPI tags.\"\n    },\n    \"hypothesis_max_examples\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"default\": 100,\n      \"description\": \"Maximum number of Hypothesis test examples to generate per operation.\"\n    },\n    \"stateful\": {\n      \"type\": \"string\",\n      \"enum\": [\"none\", \"links\"],\n      \"default\": \"none\",\n      \"description\": \"Stateful testing mode. 'links' follows OpenAPI Links for multi-step workflow testing.\"\n    },\n    \"output_sanitize\": {\n      \"type\": \"boolean\",\n      \"default\": true,\n      \"description\": \"Whether to sanitize sensitive data in test output and reports.\"\n    },\n    \"junit_xml\": {\n      \"type\": \"string\",\n      \"description\": \"File path for JUnit XML output.\"\
  \n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schemathesis/refs/heads/main/json-schema/schemathesis-config-schema.json
tags:
- API Testing
- Contract Testing
- Fuzzing
- OpenAPI
- Property-Based Testing
- Schemathesis
title: Schemathesis Configuration
---
