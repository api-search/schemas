---
description: The PUT Request JSON for HTTP Header Logging.
layout: schema
name: header-logging-put
properties_list:
- description: Whether to enable HTTP Header logging.
  name: allowSampling
  type: boolean
- description: Settings for cookie headers.
  name: cookies
  type: object
- description: Settings for custom headers.
  name: customHeaders
  type: object
- description: Settings for standard headers.
  name: standardHeaders
  type: object
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-header-logging-put-schema.json
slug: api-security-header-logging-put
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-header-logging-put-schema.json\",\n  \"title\": \"header-logging-put\",\n  \"description\": \"The PUT Request JSON for HTTP Header Logging.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowSampling\": {\n      \"description\": \"Whether to enable HTTP Header logging.\",\n      \"type\": \"boolean\"\n    },\n    \"cookies\": {\n      \"additionalProperties\": false,\n      \"description\": \"Settings for cookie headers.\",\n      \"properties\": {\n        \"type\": {\n          \"description\": \"Use `all` to log headers for all requests with any standard header. Use `none` to exclude headers for any requests with any standard header from logging. Use `exclude` to exclude headers for requests with specific standard headers. Use `only` to include headers for requests with specific\
  \ standard headers.\",\n          \"enum\": [\n            \"all\",\n            \"none\",\n            \"exclude\",\n            \"only\"\n          ],\n          \"type\": \"string\"\n        },\n        \"values\": {\n          \"description\": \"List of headers to include or exclude depending on the `type` setting.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"type\": \"array\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ],\n      \"type\": \"object\",\n      \"x-akamai\": {\n        \"file-path\": \"schemas/logging-header-setting.yaml\"\n      }\n    },\n    \"customHeaders\": {\n      \"additionalProperties\": false,\n      \"description\": \"Settings for custom headers.\",\n      \"properties\": {\n        \"type\": {\n          \"description\": \"Use `all` to log headers for all requests with any standard header. Use `none` to exclude headers for any requests with any standard header from logging. Use `exclude`\
  \ to exclude headers for requests with specific standard headers. Use `only` to include headers for requests with specific standard headers.\",\n          \"enum\": [\n            \"all\",\n            \"none\",\n            \"exclude\",\n            \"only\"\n          ],\n          \"type\": \"string\"\n        },\n        \"values\": {\n          \"description\": \"List of headers to include or exclude depending on the `type` setting.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"type\": \"array\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ],\n      \"type\": \"object\",\n      \"x-akamai\": {\n        \"file-path\": \"schemas/logging-header-setting.yaml\"\n      }\n    },\n    \"standardHeaders\": {\n      \"additionalProperties\": false,\n      \"description\": \"Settings for standard headers.\",\n      \"properties\": {\n        \"type\": {\n          \"description\": \"Use `all` to log headers for all requests with\
  \ any standard header. Use `none` to exclude headers for any requests with any standard header from logging. Use `exclude` to exclude headers for requests with specific standard headers. Use `only` to include headers for requests with specific standard headers.\",\n          \"enum\": [\n            \"all\",\n            \"none\",\n            \"exclude\",\n            \"only\"\n          ],\n          \"type\": \"string\"\n        },\n        \"values\": {\n          \"description\": \"List of headers to include or exclude depending on the `type` setting.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"type\": \"array\"\n        }\n      },\n      \"required\": [\n        \"type\"\n      ],\n      \"type\": \"object\",\n      \"x-akamai\": {\n        \"file-path\": \"schemas/logging-header-setting.yaml\"\n      }\n    }\n  },\n  \"required\": [\n    \"allowSampling\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-header-logging-put-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: header-logging-put
---
