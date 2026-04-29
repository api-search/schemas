---
description: DeliverabilityStatistics schema from AhaSend API
layout: schema
name: DeliverabilityStatistics
properties_list:
- description: Start time of the statistics bucket
  name: from_timestamp
  type: string
- description: End time of the statistics bucket
  name: to_timestamp
  type: string
- description: Number of messages accepted for delivery
  name: reception_count
  type: integer
- description: Number of messages delivered
  name: delivered_count
  type: integer
- description: Number of messages deferred
  name: deferred_count
  type: integer
- description: Number of messages bounced
  name: bounced_count
  type: integer
- description: Number of messages failed
  name: failed_count
  type: integer
- description: Number of messages suppressed
  name: suppressed_count
  type: integer
- description: Number of messages opened at least once
  name: opened_count
  type: integer
- description: Number of messages that have at least one link in them clicked.
  name: clicked_count
  type: integer
provider_name: AhaSend
provider_slug: ahasend
schema_file: json-schema/openapi-v2-deliverability-statistics-schema.json
slug: openapi-v2-deliverability-statistics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-deliverability-statistics-schema.json\",\n  \"title\": \"DeliverabilityStatistics\",\n  \"description\": \"DeliverabilityStatistics schema from AhaSend API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Start time of the statistics bucket\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"to_timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"End time of the statistics bucket\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"reception_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages accepted for delivery\",\n      \"example\": 1\n    },\n    \"delivered_count\": {\n     \
  \ \"type\": \"integer\",\n      \"description\": \"Number of messages delivered\",\n      \"example\": 1\n    },\n    \"deferred_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages deferred\",\n      \"example\": 1\n    },\n    \"bounced_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages bounced\",\n      \"example\": 1\n    },\n    \"failed_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages failed\",\n      \"example\": 1\n    },\n    \"suppressed_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages suppressed\",\n      \"example\": 1\n    },\n    \"opened_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages opened at least once\",\n      \"example\": 1\n    },\n    \"clicked_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of messages that have at least one link in them clicked.\",\n      \"\
  example\": 1\n    }\n  },\n  \"required\": [\n    \"from_timestamp\",\n    \"to_timestamp\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ahasend/refs/heads/main/json-schema/openapi-v2-deliverability-statistics-schema.json
tags:
- Email
- Transactional Email
- Developer Tools
- SMTP
- Webhooks
title: DeliverabilityStatistics
---
