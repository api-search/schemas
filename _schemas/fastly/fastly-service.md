---
description: A Fastly service represents the configuration for a website, app, API, or anything else to be served through Fastly's global edge network. Services are the primary organizational unit in Fastly, containing domain mappings, backend configurations, and VCL or Compute logic.
layout: schema
name: Fastly Service
properties_list:
- description: The alphanumeric string identifying the service.
  name: id
  type: string
- description: The name of the service.
  name: name
  type: string
- description: The alphanumeric string identifying the customer account that owns the service.
  name: customer_id
  type: string
- description: A freeform descriptive note about the service.
  name: comment
  type: string
- description: The type of service, either VCL for traditional Varnish-based services or wasm for Compute services.
  name: type
  type: string
- description: The currently active version number for the service.
  name: active_version
  type:
  - integer
  - 'null'
- description: A list of version objects associated with the service.
  name: versions
  type: array
- description: The date and time in ISO 8601 format when the service was created.
  name: created_at
  type: string
- description: The date and time in ISO 8601 format when the service was last updated.
  name: updated_at
  type: string
- description: The date and time in ISO 8601 format when the service was deleted, or null if not deleted.
  name: deleted_at
  type:
  - string
  - 'null'
provider_name: fastly
provider_slug: fastly
schema_file: json-schema/fastly-service-schema.json
slug: fastly-service
source_filename: fastly-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/fastly/service.json\",\n  \"title\": \"Fastly Service\",\n  \"description\": \"A Fastly service represents the configuration for a website, app, API, or anything else to be served through Fastly's global edge network. Services are the primary organizational unit in Fastly, containing domain mappings, backend configurations, and VCL or Compute logic.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"customer_id\", \"type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The alphanumeric string identifying the service.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the service.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"customer_id\": {\n      \"type\": \"string\",\n      \"description\": \"The alphanumeric string identifying the\
  \ customer account that owns the service.\"\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"A freeform descriptive note about the service.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of service, either VCL for traditional Varnish-based services or wasm for Compute services.\",\n      \"enum\": [\"vcl\", \"wasm\"]\n    },\n    \"active_version\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"The currently active version number for the service.\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"A list of version objects associated with the service.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ServiceVersion\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time in ISO 8601 format when the service was created.\"\n    },\n    \"updated_at\": {\n      \"\
  type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time in ISO 8601 format when the service was last updated.\"\n    },\n    \"deleted_at\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"The date and time in ISO 8601 format when the service was deleted, or null if not deleted.\"\n    }\n  },\n  \"$defs\": {\n    \"ServiceVersion\": {\n      \"type\": \"object\",\n      \"description\": \"A version of a Fastly service representing a distinct configuration snapshot that can be activated or deactivated independently.\",\n      \"required\": [\"number\", \"service_id\"],\n      \"properties\": {\n        \"number\": {\n          \"type\": \"integer\",\n          \"description\": \"The version number.\",\n          \"minimum\": 1\n        },\n        \"service_id\": {\n          \"type\": \"string\",\n          \"description\": \"The alphanumeric string identifying the service.\"\n        },\n\
  \        \"active\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version is currently active and serving traffic.\"\n        },\n        \"locked\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version is locked and cannot be modified.\"\n        },\n        \"deployed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version has been deployed.\"\n        },\n        \"staging\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version is in the staging environment.\"\n        },\n        \"testing\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this version is in the testing environment.\"\n        },\n        \"comment\": {\n          \"type\": \"string\",\n          \"description\": \"A freeform descriptive note about the version.\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\"\
  : \"date-time\",\n          \"description\": \"The date and time the version was created.\"\n        },\n        \"updated_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the version was last updated.\"\n        },\n        \"deleted_at\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"date-time\",\n          \"description\": \"The date and time the version was deleted.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fastly/refs/heads/main/json-schema/fastly-service-schema.json
tags: []
title: Fastly Service
---
