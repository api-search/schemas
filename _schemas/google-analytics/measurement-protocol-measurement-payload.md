---
description: MeasurementPayload schema from Google Analytics API
layout: schema
name: MeasurementPayload
properties_list:
- description: Uniquely identifies a user instance of a web client. Required for web streams.
  name: client_id
  type: string
- description: Uniquely identifies a user instance of an app. Required for app streams.
  name: app_instance_id
  type: string
- description: A unique identifier for a user. Enables cross-platform analysis. Must contain only UTF-8 characters.
  name: user_id
  type: string
- description: Unix timestamp in microseconds for the request. Used to backdate events up to 72 hours.
  name: timestamp_micros
  type: integer
- description: User-scoped properties for the measurement.
  name: user_properties
  type: object
- description: User-provided data for enhanced measurement.
  name: user_data
  type: object
- description: ''
  name: consent
  type: object
- description: Deprecated. Use consent.ad_personalization instead.
  name: non_personalized_ads
  type: boolean
- description: ''
  name: user_location
  type: object
- description: IP address used to derive geographic information.
  name: ip_override
  type: string
- description: ''
  name: device
  type: object
- description: Controls validation strictness. RELAXED only rejects malformed requests. ENFORCE_RECOMMENDATIONS also rejects invalid types and exceeded limits.
  name: validation_behavior
  type: string
- description: Array of event objects. Maximum 25 events per request.
  name: events
  type: array
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/measurement-protocol-measurement-payload-schema.json
slug: measurement-protocol-measurement-payload
source_filename: measurement-protocol-measurement-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-measurement-payload-schema.json\",\n  \"title\": \"MeasurementPayload\",\n  \"description\": \"MeasurementPayload schema from Google Analytics API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"Uniquely identifies a user instance of a web client. Required for web streams.\",\n      \"example\": \"123456789.1234567890\"\n    },\n    \"app_instance_id\": {\n      \"type\": \"string\",\n      \"description\": \"Uniquely identifies a user instance of an app. Required for app streams.\",\n      \"example\": \"123456\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for a user. Enables cross-platform analysis. Must contain only UTF-8 characters.\",\n    \
  \  \"example\": \"123456\"\n    },\n    \"timestamp_micros\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Unix timestamp in microseconds for the request. Used to backdate events up to 72 hours.\",\n      \"example\": 1713355200000000\n    },\n    \"user_properties\": {\n      \"type\": \"object\",\n      \"description\": \"User-scoped properties for the measurement.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/UserPropertyValue\"\n      }\n    },\n    \"user_data\": {\n      \"type\": \"object\",\n      \"description\": \"User-provided data for enhanced measurement.\"\n    },\n    \"consent\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ad_user_data\": {\n          \"type\": \"string\",\n          \"description\": \"Consent for using user data in advertising.\",\n          \"enum\": [\n            \"GRANTED\",\n            \"DENIED\"\n          ],\n          \"example\": \"GRANTED\"\n\
  \        },\n        \"ad_personalization\": {\n          \"type\": \"string\",\n          \"description\": \"Consent for ad personalization.\",\n          \"enum\": [\n            \"GRANTED\",\n            \"DENIED\"\n          ],\n          \"example\": \"GRANTED\"\n        }\n      }\n    },\n    \"non_personalized_ads\": {\n      \"type\": \"boolean\",\n      \"description\": \"Deprecated. Use consent.ad_personalization instead.\",\n      \"deprecated\": true,\n      \"example\": true\n    },\n    \"user_location\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"city\": {\n          \"type\": \"string\",\n          \"description\": \"City name.\",\n          \"example\": \"example_value\"\n        },\n        \"region_id\": {\n          \"type\": \"string\",\n          \"description\": \"Region identifier.\",\n          \"example\": \"123456\"\n        },\n        \"country_id\": {\n          \"type\": \"string\",\n          \"description\": \"Country identifier.\"\
  ,\n          \"example\": \"123456\"\n        },\n        \"subcontinent_id\": {\n          \"type\": \"string\",\n          \"description\": \"Subcontinent identifier.\",\n          \"example\": \"123456\"\n        },\n        \"continent_id\": {\n          \"type\": \"string\",\n          \"description\": \"Continent identifier.\",\n          \"example\": \"123456\"\n        }\n      }\n    },\n    \"ip_override\": {\n      \"type\": \"string\",\n      \"description\": \"IP address used to derive geographic information.\",\n      \"example\": \"123456\"\n    },\n    \"device\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Device category (e.g., mobile, tablet, desktop).\",\n          \"example\": \"example_value\"\n        },\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"Device language setting.\",\n          \"example\": \"example_value\"\n   \
  \     },\n        \"screen_resolution\": {\n          \"type\": \"string\",\n          \"description\": \"Screen resolution (e.g., 1920x1080).\",\n          \"example\": \"example_value\"\n        },\n        \"operating_system\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system name.\",\n          \"example\": \"example_value\"\n        },\n        \"operating_system_version\": {\n          \"type\": \"string\",\n          \"description\": \"Operating system version.\",\n          \"example\": \"example_value\"\n        },\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"Device model.\",\n          \"example\": \"example_value\"\n        },\n        \"brand\": {\n          \"type\": \"string\",\n          \"description\": \"Device brand.\",\n          \"example\": \"example_value\"\n        },\n        \"browser\": {\n          \"type\": \"string\",\n          \"description\": \"Browser name.\",\n          \"example\"\
  : \"example_value\"\n        },\n        \"browser_version\": {\n          \"type\": \"string\",\n          \"description\": \"Browser version.\",\n          \"example\": \"example_value\"\n        }\n      }\n    },\n    \"validation_behavior\": {\n      \"type\": \"string\",\n      \"description\": \"Controls validation strictness. RELAXED only rejects malformed requests. ENFORCE_RECOMMENDATIONS also rejects invalid types and exceeded limits.\",\n      \"enum\": [\n        \"RELAXED\",\n        \"ENFORCE_RECOMMENDATIONS\"\n      ],\n      \"default\": \"RELAXED\",\n      \"example\": \"RELAXED\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Array of event objects. Maximum 25 events per request.\",\n      \"maxItems\": 25,\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"name\"\n        ],\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name\
  \ of the event. Must not use reserved names (ad_click, app_exception, error, session_start, etc.) or reserved prefixes (_, firebase_, ga_, google_, gtag.).\",\n            \"example\": \"Example Name\"\n          },\n          \"params\": {\n            \"type\": \"object\",\n            \"description\": \"Event parameters as key-value pairs. Common parameters include session_id, engagement_time_msec, and timestamp_micros.\",\n            \"additionalProperties\": true,\n            \"properties\": {\n              \"session_id\": {\n                \"type\": \"string\",\n                \"description\": \"Session identifier for accurate session metrics.\"\n              },\n              \"engagement_time_msec\": {\n                \"type\": \"integer\",\n                \"description\": \"User engagement duration in milliseconds.\"\n              },\n              \"timestamp_micros\": {\n                \"type\": \"integer\",\n                \"format\": \"int64\",\n               \
  \ \"description\": \"Unix epoch time in microseconds to override event timestamp.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"events\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/measurement-protocol-measurement-payload-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: MeasurementPayload
---
